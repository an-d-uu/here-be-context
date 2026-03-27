# Jira to Calendar Template

Use this as a reusable template for creating Outlook calendar events from structured ICS data generated from Jira.

## Metadata

- Tool: ChatGPT (Agent Mode)
- Version: v1.0

## Overview

This template creates Outlook calendar events from structured ICS data generated from Jira.

It is designed for workflows where upstream systems, such as Jira via Rovo, have already resolved scheduling logic, and the goal is to reliably transfer that data into Outlook without reinterpretation.

The pattern emphasizes:

- trusting upstream `DTSTART` / `DTEND`
- confirming interpretation before execution
- mapping standard ICS fields into Outlook’s schema
- applying post-creation enrichment, such as category assignment

This is not a scheduling engine.  
It is a controlled handoff.

## Instructions

Before creating the event:

- Confirm the start and end time that will be used (America/Chicago)
- Confirm that `DTSTART` and `DTEND` from the ICS are being used as the event time

Then create an Outlook calendar event using the ICS data below with these rules:

Use:

- `DTSTART` / `DTEND` for the event start and end time
- `SUMMARY` as the event title
- `DESCRIPTION` as the event body
- `LOCATION`, if present
- `URL`, if present
- Include a 15-minute reminder

After creating the event:

- Assign the Outlook category `Andy Work`
- If the category does not exist, create it and then assign it

## ICS Data

[paste ICS here]
