# FLH Knowledge Base Governance

Version: 0.1.0

## Scope

Applies to FLH agent knowledge bases used by Claude (default), Codex, and Gemini.

## Layer contract

- `raw/`: immutable source material
- `wiki/`: compiled knowledge
- `index.md`: thin navigation layer
- `log.md`: append-only timeline

## Rules

- `raw/` is append-only.
- `wiki/` is synthesis, not copy-paste.
- `index.md` stays thin and content-oriented.
- `log.md` stays chronological and append-only.
- Conflicts must be marked explicitly.

## Sharing levels

- Personal KB: personal use only.
- Team KB: requires team leader approval.
- Department KB: requires departmental governance owner.
- Company KB: requires owner, audit, and release flow.

## Platform note

- Claude (default), Codex, and Gemini all follow the same KB layer contract.
