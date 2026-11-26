# ADR-005 Good-enough models

**Status:** Adopted

## Context

Running 30 agents every day on the most powerful model is expensive and usually unnecessary. Most marketing jobs don't need maximum intelligence.

## Decision

The bar for each agent is "a bit better than a very good human at this job." Any agent that meets that bar on a smaller, cheaper model runs on the smaller model. The big model is kept for work that really needs it.

## Consequences

- Much lower running costs for the same output
- Quality issues get solved with clearer job briefs, not bigger models. Most of my early failures were vague instructions, not weak models.
