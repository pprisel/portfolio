# PM-003 Agents that cried wolf

**Severity:** Medium · **Area:** Agent operations

## What happened

The agent team reported more problems than really existed. One site was flagged as missing its form, twice, when the form was working. Alerts were spread over too many Slack channels, and I spent my day checking alarms instead of building.

## Root cause

- Agents reported what they suspected without opening the page to check
- Watcher agents had no ability to fix anything, so all they could do was raise alarms
- Too many channels, so nothing felt urgent and everything felt urgent

## What changed

- Rule: confirm before you report ([governance](../governance/agent-rules.md))
- Agents that can't fix what they find were switched off ([ADR-001](../decisions/ADR-001-switch-off-agents-that-cant-fix.md))
- Channels cut down to Ads, organic, approvals and one daily recap

## Lesson

An agent team is judged by the problems it solves, not the problems it finds.
