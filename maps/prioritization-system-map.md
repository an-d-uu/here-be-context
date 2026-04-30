# Prioritization System Map

## Purpose

This document explains how the prioritization-related sources work together.

Use it to interpret adjacent frameworks without collapsing them into one system. This map is not a replacement for the individual source documents. It exists to clarify scope, relationships, precedence, and normal usage order.

## Why This Map Exists

Several sources in this repo address related but different parts of work triage, planning, estimation, and communication.

Without a shared map, it becomes easy to blur:

* urgency with importance
* importance with effort
* prioritization with communication framing
* intake decisions with delivery planning

This document reduces that confusion.

## Source Roles

### Eisenhower Matrix Work Guide

**Primary role:** intake and response mode

Use for:

* classifying new requests
* handling interruptions
* deciding whether to do, schedule, redirect, or drop work
* evaluating meetings, side requests, and unplanned asks before accepting ownership

Do not use for:

* effort sizing
* backlog estimation
* replacing tracked priority in Jira
* retroactively justifying why something was not planned well

### Jira Priority Definitions

**Primary role:** visible urgency and impact in the work system

Use for:

* expressing operational severity or business importance
* setting expectations for how tracked issues should be handled
* communicating relative urgency inside the issue system

Do not use for:

* estimating effort
* deciding whether a request should exist at all
* treating every loud request as high priority

### Story Point Estimation Process

**Primary role:** effort, complexity, and uncertainty

Use for:

* sizing accepted work
* discussing implementation effort
* identifying when work should be broken down further
* planning execution once work is already in scope

Do not use for:

* proving urgency
* setting visible business priority
* deciding whether work belongs in the active queue

### Status Framing Lexicon

**Primary role:** communication framing for updates, shifts, and explanations

Use for:

* shaping how prioritization decisions are communicated
* reducing unnecessary alarm or follow-up questions
* keeping status language professional, controlled, and non-expansive

Do not use for:

* deciding the actual priority of work
* replacing operational judgment
* hiding meaningful risk when explicit escalation is needed

## Relationship Model

These sources operate at different layers.

### Layer 1: Intake and Triage

Use the Eisenhower guide first.

Question answered:

* What kind of thing is this, and what should happen next?

### Layer 2: System Priority

Use Jira priority after work is accepted into tracked execution.

Question answered:

* How urgent and impactful is this within the issue system?

### Layer 3: Sizing and Planning

Use story points after the work is accepted and needs delivery planning.

Question answered:

* How large, complex, or uncertain is this work?

### Layer 4: Communication

Use the status-framing lexicon when describing decisions, movement, delays, or reprioritization.

Question answered:

* How should this be communicated clearly without adding unnecessary panic, noise, or implied commitments?

## Standard Operating Sequence

Use the sources in this order unless there is a clear reason not to:

1. **Eisenhower Matrix Work Guide**

   * Classify the request or interruption
   * Decide whether to do, schedule, redirect, or drop it

2. **Jira Priority Definitions**

   * If the work is accepted into tracked work, assign or interpret visible urgency and impact

3. **Story Point Estimation Process**

   * If the work will be planned or executed, size the effort, complexity, and uncertainty

4. **Status Framing Lexicon**

   * When communicating the result, use controlled framing that reflects the decision without creating accidental escalation

## Precedence Rules

When two sources seem related, use these rules:

### Rule 1: Intake comes before system priority

Do not assign Jira urgency to work that has not been consciously accepted.

### Rule 2: Priority does not define effort

A high-priority item may still be small, medium, or large.

### Rule 3: Effort does not define importance

A large story is not automatically more important than a small blocker.

### Rule 4: Communication follows judgment

Use the status-framing lexicon after deciding what is true, not instead of deciding what is true.

### Rule 5: Loud is not a category

A request being visible, recent, emotionally worded, or chat-based does not by itself determine quadrant, priority, or estimate.

## Anti-Confusion Notes

Keep these distinctions explicit:

* **Urgent** is not the same as **important**.
* **Important** is not the same as **high effort**.
* **High effort** is not the same as **high priority**.
* **Tracked** is not the same as **worth doing**.
* **Well-phrased** is not the same as **correctly prioritized**.

## Common Collision Patterns

### Collision 1: A loud same-day request arrives in chat

Use Eisenhower first.

Ask:

* What happens if this waits?
* Is there real impact?
* Does this require direct ownership here?

Only after that should Jira priority be considered.

### Collision 2: A high-priority Jira item looks small

That is normal.

Use Jira priority for urgency and impact. Use story points for size. Do not force them to match.

### Collision 3: A large story starts sounding important because it is large

Do not let size impersonate priority. Story points describe effort and uncertainty, not business value.

### Collision 4: A decision to defer work needs to be communicated cleanly

Use the status-framing lexicon to describe the decision in a controlled way after the prioritization judgment is made.

## Fast Reference

| Source                         | Main question it answers                             | Use it for                                 | Do not use it for                                   |
| ------------------------------ | ---------------------------------------------------- | ------------------------------------------ | --------------------------------------------------- |
| Eisenhower Matrix Work Guide   | What should happen next?                             | Intake, triage, response mode              | Estimation, backlog sizing, replacing Jira priority |
| Jira Priority Definitions      | How urgent and impactful is this in the work system? | Visible priority and handling expectations | Effort sizing, accepting work by default            |
| Story Point Estimation Process | How big or uncertain is this work?                   | Estimation and planning                    | Priority, urgency, value judgment                   |
| Status Framing Lexicon         | How should this be communicated?                     | Controlled status wording                  | Deciding truth, urgency, or scope                   |

## Summary

This repo contains multiple tools for different parts of work judgment. They are connected, but they are not interchangeable.

Use the Eisenhower guide to decide the response path, Jira priority to express operational urgency and impact in tracked work, story points to estimate accepted work, and the status-framing lexicon to communicate the outcome cleanly.
