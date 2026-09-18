---
title: BA harness - traceability
type: process
status: active
last_reviewed: 2026-09-18
tags:
  - business-analysis
  - traceability
---

# Traceability

## Minimum chain

```text
Goal
-> Requirement
-> Decision
-> Story
-> Acceptance criteria
-> Test
-> Outcome
```

## Record

- source of the requirement;
- relationships and dependencies;
- approval status;
- implementation status;
- test evidence;
- change history;
- outcome measurement.

Use stable IDs and WikiLinks. Do not maintain a traceability matrix that is
never used for change impact or verification.

## Agent use

The agent can find missing links, orphan requirements, impacted artifacts,
duplicate requirements, and changes without downstream review.

## Gate

Pass when a requirement can be traced to its source, decision, delivery
artifact, verification, and expected outcome.
