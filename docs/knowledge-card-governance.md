# FLH Knowledge Card Governance

Version: 0.1.0

## Scope

Applies to short, reusable agent knowledge cards that may later be promoted into FLH governance docs, training material, or published repo examples.

This policy applies to cards created by Claude (default), Codex, and Gemini.

## Purpose

- Capture one small reusable idea per card
- Keep task-local notes easy to scan
- Provide a clean promotion path from working notes to published guidance

## Card Contract

- One card = one topic
- Keep it short and operational
- Include metadata for share state and provenance
- Avoid turning a card into a long article

Recommended fields:

- `title`
- `shared`
- `shared_at`
- `shared_to`
- `created_at`
- `updated_at`
- `tags`
- `source`

Recommended filename:

- `YYYY-MM-DD-topic.md`

## Lifecycle

```text
draft → shared → promoted
```

- `draft`: task-local working note
- `shared`: sent to a person, channel, or team
- `promoted`: accepted into canonical governance docs or published examples

## Promotion Rule

A card may be promoted only if it meets all of the following:

- It is short and single-topic
- It expresses a reusable rule, heuristic, or guardrail
- It does not expose sensitive information
- It has a clear source or provenance
- It is stable enough to survive beyond the originating task

If a card is still exploratory, keep it in the task workspace and do not promote it yet.

## Sharing Levels

- Personal: keep in task-local workspace
- Team: share in a team channel or team-owned repo
- Company: promote into `publishes/flh-agent-standards` or another canonical governance repo

## Source of Truth

- Task workspaces may hold drafts and experiments
- `publishes/flh-agent-standards` holds the stable policy and promotion rules
- The published repo does not replace raw task artifacts; it curates what should outlive the task

