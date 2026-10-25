# Shared project memory

These documents let a contributor understand the current state without reconstructing the founding chat.

| File | Responsibility |
| --- | --- |
| [STATUS.md](STATUS.md) | Current facts, unknowns, and active work |
| [WORK-LOG.md](WORK-LOG.md) | Appendable task start/finish index with linked records |
| [tasks/AFS-0001-foundation.md](tasks/AFS-0001-foundation.md) | First bounded task record and its actual outcome |
| [DECISIONS.md](DECISIONS.md) | Scoped operator decisions and implementation choices |
| [HANDOFF.md](HANDOFF.md) | Latest concise continuation context |
| [BACKLOG.md](BACKLOG.md) | Proposed next tasks and dependencies |

## Start and finish

At start, read current main, status, decisions, and the relevant charter. Choose an unused task ID, create a task record from the [work-entry template](../templates/WORK-ENTRY.md), and add an active row to the log. Record the request, owner, branch, write scope, dependencies, and intended output. A log entry coordinates work; it is not a lock or permission grant.

At finish, update that task record with output links, verified findings, checks actually run, decisions, unresolved issues, and next-owner needs. Mark it completed, paused, blocked, or abandoned as appropriate. Update shared status/handoff only for material changes. Keep the log short; detail belongs in linked files and Git history.

Parallel contributors should use distinct task files and minimize edits to shared registers. Reconcile their changes through the normal branch/review workflow. Never discard another person's findings or a competing interpretation to resolve a merge conflict.

## Permissions and scope

Tasks record what the operator requested. A department title, proposed backlog item, or handoff does not authorize spawning agents, continuing studies, spending, outreach, posting, deployment, land acquisition, or background work. Use the operator's current instructions. Finish the requested scope and stop.
