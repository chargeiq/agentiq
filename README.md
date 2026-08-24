# agentiq

Cross-repo conventions for how chargeIQ's dev team and coding agents work together. Consumed as a git submodule, mounted at `/agentiq/` in each project repo.

## Scope

This repo holds chargeIQ-specific policy only — the things that are true across our repos but aren't generic software-engineering practice (that layer is each developer's own machine-wide agent skill set, e.g. `~/.claude/skills/`, and isn't duplicated here). See [`CONVENTIONS.md`](CONVENTIONS.md).

Not (yet) in scope: enforcement hooks, a forked copy of generic skills, general reference material. Those are separate decisions to make if and when a concrete need shows up — see `help-agent-prototype`'s `docs/adr/0003-agentiq-shared-conventions-repo.md` for the reasoning.

## Using this repo

Add as a submodule in a consuming repo:
```bash
git submodule add git@github.com:chargeiq/agentiq.git agentiq
```

It's editable in place — no version pinning yet:
```bash
cd agentiq/
# edit, commit, push directly to this repo's own remote
cd ..
git add agentiq && git commit   # bumps the pinned commit in the consuming repo
```

## Adding a convention

Only add a rule to `CONVENTIONS.md` once it's proven true across 2+ repos — not speculatively from a single repo's perspective. If it's only true for one repo, it belongs in that repo's own `CLAUDE.md`/`docs/`, not here.
