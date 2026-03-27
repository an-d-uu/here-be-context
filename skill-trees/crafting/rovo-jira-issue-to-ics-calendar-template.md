# Rovo Jira Issue to ICS Calendar Template

Use this as a reusable Rovo template for converting a Jira issue into `.ics` calendar content without reinterpretation of the underlying schedule data.

## Metadata

- Tool: Rovo
- Version: v1.0

## Overview

This template creates calendar appointment content from a Jira issue and outputs the result as `.ics` or `.cal` file content in a single code block.

It is designed for workflows where Jira is the source of truth for the issue, scheduling fields, comments, and linked work items, and the goal is to reliably translate that data into valid calendar content.

The pattern emphasizes:

- trusting upstream Jira scheduling fields
- using a deterministic start and end selection rule
- preserving raw metadata in custom X-properties
- producing a structured event description from multiple Jira fields
- emitting valid calendar content in a single code block

This is not a scheduling engine.  
It is a controlled transformation.

## Instructions

Create a calendar appointment for Jira issue `TIS-123999` and output it as `.ics` or `.cal` file content in a single code block.

### Scheduling Rule

- If `Actual start` and `Actual end` are present, use them for `DTSTART` and `DTEND`
- Otherwise use `Planned start` and `Planned end`
- Timezone must be `America/Chicago` using a `VTIMEZONE` block

### Event Fields

Use the following event field rules:

- `SUMMARY`: include the ticket summary and the key in parentheses
- `LOCATION`: `SUMWHRE WIF INTRNET`
- `STATUS`: `CONFIRMED`
- Include `URL:` pointing to the Jira browse URL for the issue
- Add `CATEGORIES:Jira,Change,Completed` if the ticket is completed; otherwise omit `Completed` or use the current status
- Add a reminder alarm using `VALARM` with:
  - `TRIGGER:-PT15M`
  - `ACTION:DISPLAY`
  - `DESCRIPTION:Reminder - <KEY>`

### Custom Metadata

Add the following custom X-properties even if the calendar client does not display them:

- `X-TYLER-JIRA-STATUS:<status>`
- `X-TYLER-PLANNED-START:<planned start raw value>`
- `X-TYLER-PLANNED-END:<planned end raw value>`
- `X-TYLER-ACTUAL-START:<actual start raw value if present>`
- `X-TYLER-ACTUAL-END:<actual end raw value if present>`

### DESCRIPTION Formatting

Merge the following sections into `DESCRIPTION` in this exact order:

1. `Description`
2. `Implementation plan`
3. `Test plan`
4. `Backout plan`
5. `Linked Work Items`
   - Format each as: `<KEY>: <URL>`
   - The URL text should display as the project key, such as `TIS-123456`, and the address should be the full issue URL
6. `All Comments`
   - For each commenter, add a subheader line formatted exactly as:
     `Full Name: YYYY-MM-DD HH:MM:SS ±ZZZZ`
   - Then include the comment body beneath it

## Output Requirements

- Output the calendar content in a single code block
- After the code block, include a `Sources` section
- In the `Sources` section, include the Jira issue URL
