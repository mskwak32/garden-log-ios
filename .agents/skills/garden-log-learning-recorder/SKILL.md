---
name: garden-log-learning-recorder
description: Close a completed Garden Log iOS work unit by writing its single durable work-unit learning note and rolling project records forward. Use only for work-unit completion, not routine progress updates.
---

# Garden Log Learning Recorder

Convert a verified completed unit into concise material that remains useful after the implementation details are forgotten.

## Confirm Completion

1. Read `AGENTS.md`, `docs/project-plan.md`, `docs/work-status.md`, and the relevant project files.
2. Confirm the active unit's agreed outcome with appropriate evidence.
3. If required work or verification remains, report it and stop without closing the unit.

## Record Durable Learning

1. Extract the concepts, decisions, and meaningful problem/cause/solution details from the completed work.
2. Create or update exactly one `docs/learning/NN-work-unit-title.md` file for the completed unit, using `docs/learning/_template.md` as guidance.
3. Keep all concepts learned in that unit in the same document, using separate `###` headings under `## 배운 내용`.
4. Keep multiple meaningful problems in the same document, using one `###` section per problem under `## 문제와 해결`.
5. Explain what each concept is, why it matters, how it applies here, and where the Android analogy stops.
6. Use a small representative example when it improves recall.

Exclude chronology, progress checklists, exhaustive final code, commit summaries, changed-file inventories, and trivial problems. Omit empty sections instead of filling them mechanically.

## Close the Unit

1. Update `docs/system-architecture.md` only when the completed unit established a confirmed cross-cutting decision.
2. Mark the unit complete in `docs/project-plan.md`.
3. Replace `docs/work-status.md` with a short no-active-unit state. Do not select the next unit for the user.

## Boundaries

- Do not close a unit based only on an implementation claim; require proportionate verification.
- Do not create separate learning documents for individual concepts within one work unit.
- Do not include planned architecture as confirmed architecture.
- Do not sync to Notion unless separately requested and configured.
- Do not add tests solely because a unit is being closed.
