# Change Policy

This document defines how the System Momentum Canon may change.

The Canon is not a document that evolves by habit.
It changes only through explicit, constrained action.

---

## Scope

This policy governs changes to:

- `canon/`
- `governance/`
- `STATUS.md`
- `versions/`

It does not govern derivative artifacts or implementations.

---

## Change Principles

1. **Explicitness**  
   All changes must be explicit and traceable.  
   There is no implicit evolution.

2. **Hierarchy Preservation**  
   Changes must respect the canonical hierarchy.  
   Lower-level artifacts must not force changes upward.

3. **Integrity Over Convenience**  
   Changes that improve readability must not weaken constraints.  
   Convenience is not a justification.

4. **No Retroactive Legitimization**  
   Canonical violations cannot be legitimized by later edits.  
   Fixing ambiguity is permitted; rewriting history is not.

---

## Allowed Change Types (v0.x)

The following changes are permitted during v0.x:

- removing ambiguity
- eliminating internal inconsistency
- tightening definitions
- strengthening constraints
- clarifying prohibited patterns
- improving structural precision without expanding scope

---

## Prohibited Change Types

The following changes are prohibited:

- expanding scope without explicit version intent
- introducing implementation-specific dependencies
- weakening invariants, constraints, or non-negotiables
- reframing the Canon as a product/spec/manifesto
- introducing consensus-driven authority
- adding “best practices” or advisory guidance as if canonical

---

## Version Semantics

- **v0.x**  
  The Canon is defined but unstable.  
  Breaking changes are permitted. Backward compatibility is not guaranteed.

- **v1.0**  
  Stability requires explicit declaration.  
  Breaking changes require a new major version.

Versioning is declared in `STATUS.md` and recorded in `versions/`.

---

## Change Mechanics

1. **One change per commit**  
   Each commit must represent a single canonical intent.

2. **No amend / rewrite**  
   History is not rewritten. Corrections are new commits.

3. **Commit messages must be declarative**  
   Example: `canon: tighten definition of validity`  
   Not: `fix stuff` or `updates`.

4. **Status updates are mandatory when meaning changes**  
   If canonical meaning shifts, `STATUS.md` must reflect it.

---

## Canonical Review Standard

A change is acceptable only if:

- it does not contradict `canon/01-canonical-hierarchy.md`
- it does not violate scope boundaries in `canon/02-scope-and-non-goals.md`
- it preserves or strengthens constraints and non-negotiables
- it reduces ambiguity without expanding interpretation space

---

## Declaration

This policy is binding.

Deviation requires explicit policy change.
Implicit reinterpretation is prohibited.
