# FLH Agent Skill Governance

Version: 0.1.0

## Scope

Applies to all FLH agent skill packages used by Claude (default), Codex, and Gemini.

## Rules

- Skill name is canonical and shared across platform adapters.
- Each package keeps one canonical README plus per-platform manifests when needed.
- `metadata.version` is the source of truth for versioning.
- `metadata.author` is the primary maintainer.
- A skill can be `draft`, `active`, `deprecated`, or `retired`.
- `deprecated` means no active maintenance, but existing users may still transition.

## Sharing levels

- Personal: local scope, no review required.
- Workspace: repo-managed shared scope, requires team leader audit.
- Company: release artifact / published package, requires release flow and changelog.

## Platform note

- Claude (default) is the primary authoring and review surface.
- Codex and Gemini may use different loaders, but the governance package name and version must stay aligned.
