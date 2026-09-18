---
title: BA AI Harness
type: guide
status: active
last_reviewed: 2026-09-18
tags:
  - business-analysis
  - harness
  - agent
---

# BA AI Harness

Harness is a repeatable workflow for business analysis with AI.
It controls the path from a vague request to a verified business outcome.

## Flow

```text
Intake
-> Discovery
-> Analysis
-> Requirements
-> Validation
-> Traceability
-> Decision
-> Delivery readiness
-> Outcome review
```

The work can move back to an earlier stage when new evidence appears.

## Stage index

1. [[01_Intake]]
2. [[02_Discovery]]
3. [[03_Analysis]]
4. [[04_Requirements]]
5. [[05_Validation]]
6. [[06_Traceability]]
7. [[07_Decision_and_Prioritization]]
8. [[08_Delivery_Readiness]]
9. [[09_Outcome_Review]]

## Quality gates

- `G0 Intake`: problem, goal, scope, and result are clear.
- `G1 Discovery`: stakeholders, sources, and questions are known.
- `G2 Requirements`: requirements are unambiguous and testable.
- `G3 Validation`: gaps, conflicts, and edge cases are reviewed.
- `G4 Delivery`: scope, criteria, dependencies, and risks are usable by delivery.
- `G5 Outcome`: the result is compared with the original goal.

## AI role

AI may prepare questions, summarize evidence, draft requirements, find gaps,
compare options, and check consistency.

AI must not invent stakeholder intent, approve requirements, hide uncertainty,
or replace human validation.

## Minimal task packet

```text
Context:
Goal:
Problem:
Sources:
Stakeholders:
Constraints:
Expected output:
Validation criteria:
```

Use the skills in `.cursor/skills/` for repeatable agent workflows.
