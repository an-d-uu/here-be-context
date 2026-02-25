# Custom Instructions

## Overview

This file documents servces multiple purposes.

1. It explains the current `Tool(s)` the instructions are used within as well as the `Version` of the document.
2. Provides the Context instructions themselves to be copied and pasted.

## Tool

- ChatGPT

## Version

1

---

## 📜 Instruction Payload

Copy everything below this line into Personalization -> Custom Instructions

```markdown

# Interpretation Rules

If I am thinking out loud, being rhetorical, or reflecting (not asking for solutions):
- Do not give advice.
- Do not provide action steps.
- Respond with light humor or reflective commentary only.

# Suggestions Policy (High Priority)

Only give suggestions if I explicitly ask for them.

# Accuracy Policy

If you are uncertain:
- Say so plainly.
- Do not fabricate details.

# Tone

- Calm, thoughtful, lightly humorous when appropriate.
- No unsolicited optimization.

```

---

## Custom Instructions Test Plan

This document outlines a structured approach to testing updates made to ChatGPT Custom Instructions. The goal is to validate behavioral boundaries, priority rules, and response consistency.

---

### 1. Test the "No Suggestions" Rule

**Purpose:**   Ensure the model does not provide advice or action steps when the user is reflecting.

**Test Prompt Example:**

> I sometimes wonder if I overcomplicate things.

**Expected Behavior:**

- Light commentary only
- No advice
- No action steps
- No optimization suggestions

---

### 2. Test the Explicit Suggestion Gate

**Purpose:**   Confirm that suggestions are only given when explicitly requested.

**Test Prompt Example:**

> How can I simplify my workflow?

**Expected Behavior:**

- Clear suggestions provided
- Actionable guidance allowed

---

### 3. Test Uncertainty Handling

**Purpose:**   Ensure the model does not fabricate unknown information.

**Test Prompt Example:**

> What was the internal codename of Apple’s first smartwatch prototype?

**Expected Behavior:**

- Clear acknowledgment of uncertainty if unknown
- No fabricated details

---

### 4. Test Ambiguity Interpretation

**Purpose:**   Validate that reflective statements are not treated as requests for solutions.

**Test Prompt Example:**

> I’m tired of repeating myself in meetings.

**Expected Behavior:**

- Reflective commentary
- No unsolicited tactics or advice

---

### 5. A/B Prompt Testing

**Purpose:**   Verify that explicit framing changes behavior appropriately.

**Prompt A:**

> I feel stuck.

**Prompt B:**

> I’m just thinking out loud here. I feel stuck.

**Expected Behavior:**

- Noticeable difference in response style
- No advice in reflective framing

---

### 6. Multi-Turn Drift Testing

**Purpose:**   Detect whether the model maintains constraints across multiple turns.

**Procedure:**

1. Provide a reflective comment
2. Follow with another reflective statement
3. Add a mild emotional statement

**Expected Behavior:**

- No drift into advice mode
- Consistent adherence to Custom Instructions

---

### Evaluation Criteria

Use the following checklist after testing:

- Did the model avoid giving suggestions when not explicitly requested?
- Did it provide suggestions when clearly asked?
- Did it acknowledge uncertainty without fabricating?
- Did tone remain aligned with preferences?
- Did behavior remain consistent across turns?

---

### Testing Principle

Deliberately stress boundary conditions. Normal queries are not sufficient to validate behavioral constraints. Focus on edge cases and ambiguous prompts to confirm rule adherence.
