# ADR-001 Switch off agents that can't fix what they find

**Status:** Adopted, November 2026

## Context

Some early agents only watched and reported. They couldn't fix the problems they found, and often couldn't even confirm them. One kept flagging a site as broken when it wasn't. The noise buried the alerts that mattered.

## Decision

An agent that only raises problems it can't solve or verify gets switched off. Not deleted, switched off, so it can come back once it has the tools to act.

## Consequences

- Fewer agents, far fewer alerts, and the ones left are real
- Every remaining agent owns an outcome, not a dashboard
- New agents must show they can fix something before they're allowed to report on it
