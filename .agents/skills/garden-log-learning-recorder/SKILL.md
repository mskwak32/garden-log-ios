---
name: garden-log-learning-recorder
description: Close a completed Garden Log iOS work unit by writing durable topic-based learning notes and rolling project records forward. Use only for work-unit completion, not routine progress updates.
---

# Garden Log Learning Recorder

Convert a verified completed unit into concise material that remains useful after the implementation details are forgotten.

## Confirm Completion

1. Read `AGENTS.md`, `docs/project-plan.md`, `docs/work-status.md`, and the relevant project files.
2. Confirm the active unit's agreed outcome with appropriate evidence.
3. If required work or verification remains, report it and stop without closing the unit.

## Record Durable Learning

1. Extract the concepts, decisions, and meaningful problem/cause/solution details from the completed work.
2. Create or update one focused `docs/learning/NN-topic.md` file using `docs/learning/_template.md` as guidance.
3. Split notes only when the topics are likely to be searched independently later.
4. Explain what each concept is, why it matters, how it applies here, and where the Android analogy stops.
5. Use a small representative example when it improves recall.

Exclude chronology, progress checklists, exhaustive final code, commit summaries, changed-file inventories, and trivial problems. Omit empty sections instead of filling them mechanically.

## Close the Unit

1. Update `docs/system-architecture.md` only when the completed unit established a confirmed cross-cutting decision.
2. Mark the unit complete in `docs/project-plan.md`.
3. Replace `docs/work-status.md` with a short no-active-unit state. Do not select the next unit for the user.

## Boundaries

- Do not close a unit based only on an implementation claim; require proportionate verification.
- Do not include planned architecture as confirmed architecture.
- Do not sync to Notion unless separately requested and configured.
- Do not add tests solely because a unit is being closed.
