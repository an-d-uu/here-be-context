# Eisenhower Matrix for My Work

## Purpose

Use this document as a lightweight intake and prioritization guide for tasks, requests, interruptions, and meetings.

This framework is meant to help classify work before reacting to it. It is not a replacement for Jira priorities, story points, sprint planning, or existing delivery commitments.

## What This Framework Is For

Use this guide when:

* a new task appears
* someone asks for a quick favor
* a meeting invite arrives without clear value
* an issue feels urgent but the actual impact is unclear
* multiple competing requests need a response path

Do not use this guide as the sole source of truth for delivery sequencing, estimation, or backlog management.

## Core Definitions

### Urgent

A task is urgent when delay creates a near-term consequence.

Examples:

* active blocker with no practical workaround
* same-day or next-day deadline with real impact
* production or workflow disruption requiring prompt action
* dependency that will immediately stall other work

Urgent does not mean:

* someone marked it high priority without context
* the request arrived in chat instead of Jira
* the sender wants a fast answer
* the work feels noisy or emotionally loaded

### Important

A task is important when it materially affects goals, commitments, customers, delivery, quality, risk, or team effectiveness.

Examples:

* work tied to delivery commitments or business outcomes
* issues that affect customers, compliance, data integrity, or system reliability
* work that prevents repeated problems or reduces future operational drag
* planning, documentation, or process improvements that meaningfully improve execution

Important does not mean:

* interesting
* visible
* politically loud
* easy to justify after the fact

## The Four Response Paths

### 1. Do First

Use when work is both urgent and important.

Typical examples:

* blocker with no workaround
* production issue or major disruption
* deadline-driven work with real downstream impact
* issue that prevents others from proceeding

Default response:

* engage now
* reduce ambiguity quickly
* communicate only the context needed for alignment
* move into the active queue immediately

### 2. Schedule

Use when work is important but not urgent.

Typical examples:

* planning and design work
* documentation that reduces repeat questions or rework
* technical debt with real delivery or support impact
* process improvements
* preparation work that supports future delivery

Default response:

* place intentionally into backlog, sprint planning, or a scheduled work block
* avoid treating this as filler work for spare minutes
* protect it from being displaced by low-value urgency

### 3. Delegate or Redirect

Use when work is urgent to someone, but does not require this role, this context, or this ownership.

Typical examples:

* routing questions
* administrative asks
* requests better handled by another function, owner, or teammate
* meeting coordination and information gathering that does not require direct involvement

Default response:

* redirect to the right owner
* delegate when appropriate
* clarify the handoff point
* avoid partial ownership that turns into hidden follow-up work

### 4. Decline, Defer, or Drop

Use when work is neither urgent nor important.

Typical examples:

* low-value meetings with no decision or action path
* requests with no meaningful outcome
* duplicated reporting or status churn
* nice-to-have work with no current value
* work that creates motion without progress

Default response:

* decline when appropriate
* defer without creating implied commitment
* remove from active attention

## Intake Questions

Use these questions before accepting work:

1. What happens if this waits?
2. What is the actual consequence of delay?
3. What goal, commitment, customer, risk, or dependency does this affect?
4. Does this require my role, authority, or context specifically?
5. Is this real work, coordination work, or work-about-work?
6. Is the urgency operationally real, or just socially loud?

## Mapping to Existing Tools

### Eisenhower Matrix

Use for:

* intake
* response mode
* interruption handling
* deciding whether to engage, schedule, redirect, or decline

### Jira Priority

Use for:

* visible business urgency and impact
* issue handling expectations
* communicating severity in the work system

### Story Points

Use for:

* effort
* complexity
* uncertainty
* deciding whether work should be broken down further

## Working Rules for Compatibility

To keep this framework aligned with the other sources:

* Do not use Eisenhower categories as a substitute for Jira priority labels.
* Do not use urgency as a proxy for estimation.
* Do not convert every interruption into tracked work unless it materially affects delivery, support, or accountability.
* Do not treat all important work as immediate work.
* Do not let chat-based requests bypass normal intake without a conscious decision.

## Practical Translation to Current Work

### Likely Do First

* drop-everything issues
* blockers with no workaround
* real delivery or operational disruptions

### Likely Schedule

* documentation with repeat-value
* process cleanup
* technical debt that reduces recurring friction
* planning work that protects future delivery

### Likely Delegate or Redirect

* requests lacking a clear ownership match
* coordination tasks that belong elsewhere
* asks that need access or input but not direct execution here

### Likely Decline, Defer, or Drop

* status churn with no decision value
* meetings with unclear purpose
* low-impact nice-to-have work
* requests that create hidden maintenance without meaningful outcome

## Anti-Patterns

Watch for these:

* Treating "someone asked today" as proof of urgency
* Treating "this matters eventually" as a reason to do it immediately
* Accepting ambiguous work before defining impact
* Keeping soft ownership of delegated work without agreement
* Using the framework to justify avoidance instead of prioritization
* Letting Quadrant 2 work disappear because Quadrant 3 work is louder

## Response Framing Guidance

Use neutral, scope-safe language when responding to requests.

Prefer:

* "I can help assess where this fits."
* "This looks important, but not time-critical."
* "This appears urgent for routing, but not necessarily for direct involvement here."
* "This should be scheduled rather than handled ad hoc."
* "This may be better handled by [role/team/system]."

Avoid:

* implied commitments without a decision
* emotional urgency language without operational meaning
* vague ownership language that invites follow-up work

## Examples

### Example 1: Blocking issue with no workaround

Classification: Do First

Reason: Immediate operational consequence and real delivery impact.

### Example 2: Documentation update that prevents repeat confusion

Classification: Schedule

Reason: Important because it reduces recurring friction, but not urgent unless tied to a near-term dependency.

### Example 3: Same-day request that belongs to another owner

Classification: Delegate or Redirect

Reason: Time-sensitive to someone, but not work that requires direct ownership here.

### Example 4: Nice-to-have enhancement with no current impact

Classification: Decline, Defer, or Drop

Reason: Low urgency and low present importance.

## How to Use This With ChatGPT

When discussing a task or interruption, ask for:

* classification by quadrant
* rationale for urgent vs important
* recommended response path
* draft language for redirecting, scheduling, or declining
* identification of where this conflicts with Jira priority or effort sizing

Suggested prompt:

> Classify this using my Eisenhower work guide. Tell me whether it is urgent, important, both, or neither. Then recommend whether to do, schedule, redirect, or drop it, and explain any conflict with Jira priority or story-point sizing.

## Maintenance Notes

Update this document when:

* the working definition of urgent changes
* Jira priority usage changes
* estimation practices change
* repeated edge cases show up that are not handled well here
* response-framing preferences evolve

## Summary

This framework is for deciding how to respond to work, not for replacing existing delivery systems. Use it to reduce reactive decisions, protect important work, and keep urgency from quietly becoming the default ruler of the kingdom.
