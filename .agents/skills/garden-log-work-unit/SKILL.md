---
name: garden-log-work-unit
description: Start, resume, or review the current Garden Log iOS work unit using the long-term plan and temporary status. Use for orientation and active-unit progress, not for final learning-note creation.
---

# Garden Log Work Unit

Keep the current unit focused and resumable without turning its status into a permanent diary.

## Start or Resume

1. Read `AGENTS.md`, `docs/project-plan.md`, and `docs/work-status.md`.
2. Read only the architecture and learning notes relevant to the current unit.
3. Inspect actual project files needed to verify recorded claims.
4. Summarize the unit's outcome, confirmed state, remaining work, and decisions reserved for the user.
5. Stop before implementation unless the user explicitly requested the specific change.

Continue an existing active unit across sessions. Do not create a new unit merely because a new conversation started.

## Maintain Temporary Status

Update `docs/work-status.md` only when the user requests progress recording or the requested task explicitly includes documentation maintenance. Keep only:

- the active unit and its completion criteria;
- confirmed decisions and constraints;
- completed and remaining checks;
- the next concrete question or action.

Do not preserve timestamps, conversation summaries, attempt history, commit summaries, or changed-file lists. If the current scope no longer fits one unit, explain the mismatch and propose a split or merge based on `docs/project-plan.md`; do not change the long-term plan without user approval.

## Boundaries

- Do not create final learning notes or mark a unit complete.
- Do not implement application code without explicit authorization.
- Do not infer product or architecture decisions reserved for the user.
