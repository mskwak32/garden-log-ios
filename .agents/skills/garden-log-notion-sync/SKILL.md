---
name: garden-log-notion-sync
description: Sync explicitly selected Garden Log iOS learning notes or the system architecture document to their configured Notion pages. Requires available Notion tools and user approval before every external write.
---

# Garden Log Notion Sync

Sync only durable project documentation. Never sync temporary progress or planning files.

## Destinations

- Learning-note parent, `작업 과정`: `3df6e29b97d580f3867ef8a7ed5c4dda`
- Architecture page, `아키텍쳐`: `3df6e29b97d58092b2ffc2e7f44dcb5f`

Each `docs/learning/*.md` note becomes a child page under `작업 과정`. `docs/system-architecture.md` updates the configured `아키텍쳐` page.

Exclude `docs/learning/_template.md`, `docs/work-status.md`, and `docs/project-plan.md`.

## Workflow

1. Require the user to specify `docs/system-architecture.md` or one or more concrete learning-note paths. Ask for the target when none is specified.
2. Check that suitable Notion read, create, and update tools are available. If not, stop and state that the Notion integration is required; do not install, test, or substitute another integration.
3. Verify that each local source exists and is an allowed target.
4. Read the first H1 as the page title and omit that H1 from the page body.
5. Resolve the intended action without writing:
   - Architecture always updates the configured page body and keeps its existing Notion title and parent.
   - For a learning note, search only under the configured parent for an exact title match. Update one match, create a child page when none exists, and stop for that note when multiple matches exist.
6. Show the candidate source, destination, and create/update action. Ask for explicit approval.
7. Perform only the approved writes and report each result.

## Rules

- Do not sync every note by default or expand beyond explicitly selected files.
- Do not modify local Markdown while preparing Notion content.
- Preserve useful headings, lists, tables, code blocks, and Mermaid blocks when supported; do not invent replacement diagrams or content.
- Do not create duplicate learning pages when an exact child-title match exists.
- Do not move pages, rename configured parents, or change the architecture page title.
- Do not maintain a local sync-state file.
- Stop before all external writes unless the user approved the displayed candidates in the current request flow.
