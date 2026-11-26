# ADR-004 One owner per job

**Status:** Adopted, November 2026

## Context

At one point the same job, such as Ads optimization or the daily recap, was covered by more than one agent on more than one platform. They duplicated work, contradicted each other and posted in too many channels.

## Decision

Every job has exactly one agent that owns it. If two agents could do it, one gets switched off.

## Consequences

- Clear accountability: when something is wrong, I know which agent to look at
- Slack went from a dozen agent channels to a handful
- Less token spend on duplicated runs
