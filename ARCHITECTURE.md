# ARCHITECTURE.md

This file explains the repository-level structure of `flh-agent-standards`.

It focuses on:

- why the repository is partitioned this way
- how content moves between areas
- which locations are usually the current source of truth

## Relationship To Other Root Files

- `README.md`
  overview and quick navigation
- `AGENTS.md`
  agent navigation and reading order

## Partition Model

- `docs/`
  stable governance text for FLH agent standards
- `projects/`
  GitHub Project inventory and repo tracking snapshot
- `README.md`
  repository overview and entry point
- `AGENTS.md`
  repository navigation and operating rules

## Content Lifecycle

1. Draft and working notes live upstream in task workspaces or review threads.
2. Stable governance text is promoted into `docs/`.
3. Repo inventory and project tracking live in `projects/`.
4. When rules change, update the relevant `docs/` file and record the change in the repo history.

## Source-of-Truth Heuristics

1. Start from root `AGENTS.md` and `README.md`.
2. Use `ARCHITECTURE.md` to resolve boundary questions.
3. Once inside `docs/`, follow `docs/README.md` and the specific governance document you need.
4. Use `projects/` for inventory and tracking only; do not treat it as policy text.
5. Keep upstream task workspaces as the source for drafts, examples, and unresolved decisions.

## Promotion Rules

### Task Drafts to `docs/`

Promote content when:

- the rule is stable enough to survive beyond the originating task
- the language is short, explicit, and reusable
- the rule has a clear owner or review path

### Policy Text to `projects/`

Only promote tracking data when:

- the GitHub Project item exists or changes state
- the repo inventory needs a snapshot update
- the entry helps humans and agents find the current tracking source

