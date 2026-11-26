# PM-002 The Zap that ate the quota

**Severity:** Medium · **Area:** Automation

## What happened

A Zapier workflow kept firing nonstop. It burned through the account's entire monthly task allowance, and every other automation stopped with it: lead routing, CRM updates, notifications.

## Root cause

The sync was set to run far more often than the data actually changed, with nothing watching for runaway loops.

## What changed

- Data syncs run at most once a day unless there's a real reason not to
- A watchdog audits the Zaps and alerts when one misbehaves
- New automations get a run-frequency check before they go live

## Lesson

Automation costs are invisible until they aren't. Schedule for how often the data changes, not for how fast the tool can go.
