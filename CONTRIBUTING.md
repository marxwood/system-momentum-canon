# Contributing

This repository is in **Public Draft (v0.2)**.
Contributions are welcome, but scope is intentionally constrained.

## Canonical Entry

Canonical navigation is defined exclusively in `core/INDEX.md`.

## Allowed Changes (v0.2 Draft)

- fix broken links and paths
- improve navigation and indexing without changing meaning
- correct typos and editorial mistakes
- clarify ambiguity without adding new concepts
- remove internal contradictions by tightening wording (not by expanding scope)

## Prohibited Changes

- new canonical domains or new primitives
- new authority or expanded canonical scope
- implementation guidance (code, schemas, workflows, tooling, infra)
- normative “why” narratives inside `core/`
- moving canonical meaning into repository surfaces (README, MAP, issues, PR text)

## Where Content Belongs

- `core/`: canonical meaning and invariants
- `derivatives/`: structural decompositions of canonical constructs (non-authoritative)
- `doctrines/`: human-readable operational and civilizational explanation (non-authoritative)
- `governance/`: change control and publication discipline (non-canonical)

See `governance/content-rules.md` for binding stratification rules.

## Change Discipline

- one intent per commit (see `governance/change-policy.md`)
- no history rewriting
- keep diffs minimal and local
