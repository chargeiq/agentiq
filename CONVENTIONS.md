# Conventions

Rules that apply across every chargeIQ repo, not just one. Add a rule here once it's actually proven true across 2+ repos, not speculatively.

## Precedence

When instructions conflict, resolve in this order:
1. `agentiq/CONVENTIONS.md` (this file) — cross-repo, wins over everything below.
2. The repo you're in — its own `CLAUDE.md`/`docs/` — wins over personal instructions.
3. A developer's personal/local instructions (e.g. `~/.claude/CLAUDE.md`) — narrowest scope, applies last.

## Keeping docs current

While doing work — writing code, comments, or docs — fold in what you learn:
- A fact true across chargeIQ repos belongs here, in `agentiq/`, not duplicated into one repo's docs.
- A fact true only for the repo you're in belongs in that repo's own `CLAUDE.md`/`docs/`.
- If a change makes existing prose (a comment, a doc, this file) stale, update it in the same change — don't leave it for later.

## Scope

These rules bind you while producing something — code, comments, a doc edit. A question answered in chat stays read-only: answer it, don't take it as an occasion to go edit files.
