# Canonical Authority

This document defines **where authority resides** inside the System Momentum Canon repository, and how authority propagates across artifacts.

This document is **governance**, not Canon.
It does not define canonical meaning.
It defines how canonical meaning is **referenced, protected, and applied**.

Canonical meaning is defined only by documents listed in `canon/INDEX.md`.

---

## Authority Levels

Authority is layered. Each layer may constrain layers below it, but must not be constrained by layers below it.

| Level | Artifact Class                                               | Purpose                                                                                                                       | Can Introduce New Concepts? |         Can Change Canonical Meaning? |
| ----: | ------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------- | --------------------------: | ------------------------------------: |
|     0 | **Canon** (`/canon`)                                         | Ontological and epistemic invariants. Defines what must remain true across time, orgs, and implementations.                   |             Yes (only here) | Yes (only via Canon revision process) |
|     1 | **Governance** (`/governance`, `/versions`, root policies)   | Protects Canon integrity: change control, immutability, release discipline, disclosure boundaries, and audit.                 |                          No |                                    No |
|     2 | **Derivatives** (`/derivatives`)                             | Allowed interpretations and realizations of Canon for specific contexts. Provide “theory of realization”, not execution.      | No (must derive from Canon) |                                    No |
|     3 | **System-level ADRs / PRDs** (`/adrs`, `/prds` when present) | Cross-derivative decision and requirement discipline. Normative obligations that apply broadly without binding to technology. |                          No |                                    No |
|     4 | **Derivative-scoped ADRs / PRDs** (inside a derivative)      | Local decisions and obligations within one derivative’s scope.                                                                |                          No |                                    No |
|     5 | **Implementation Repositories** (external)                   | Executable artifacts: code, infra, deployment, runtime operations.                                                            |           No (must conform) |                                    No |

Notes:

- If `adrs/` and `prds/` are not yet present at repo root, their authority level is reserved; derivative-scoped ADR/PRD discipline may still exist under `/derivatives/*`.
- “New concepts” means: introducing new primitive terms that are required to interpret Canon. Derivatives may _name_ and _compose_ Canon concepts, but must not invent new primitives.

---

## The ADR-0 / ADR-1 Mapping

The repository uses the following equivalence for cross-thread consistency:

- **ADR-0 == Canon** (authority level 0)
- **ADR-1\*** == derivative-scoped architectural decisions (authority level 4)

Implications:

- “ADR-0” is not a folder. It is a shorthand for the fact that Canon functions as the constitutional decision layer.
- There is no single ADR-1. Multiple ADR-1 decisions may exist in parallel, each scoped to a derivative.

---

## Non-Canonical Does Not Mean Optional

Many artifacts in this repository are explicitly **non-canonical** (e.g., `MAP.md`, most of `/derivatives`, governance documents).

Non-canonical means:

- the artifact does not define canonical meaning

Non-canonical does **not** mean:

- low importance
- disposable
- unconstrained by Canon

All artifacts in this repository must remain Canon-compatible unless explicitly labeled as:

- illustrative,
- experimental,
- or intentionally adversarial for testing.

---

## Directionality Rules

Directionality is a hard rule for maintaining authority boundaries.

**Allowed references**

- Derivatives MAY reference Canon.
- ADRs/PRDs MAY reference Canon and (optionally) the derivative they belong to.
- Implementation repositories MUST reference the specific Canon version and the relevant derivative + ADR/PRD set they claim to satisfy.

**Forbidden references**

- Canon MUST NOT reference Derivatives, ADRs, PRDs, or implementations.
- Derivatives MUST NOT require changes to Canon as a precondition for their validity.
- ADRs/PRDs MUST NOT redefine Canon terms or add new primitives.

---

## Canon Compliance as a Proof Obligation

Any claim of compliance must be provable by explicit references:

Minimum proof set for an implementation (external repo):

1. Canon version (e.g., tag/release or `versions/*`)
2. Derivative scope (which derivative applies)
3. ADR set (system-level + derivative-scoped, as applicable)
4. PRD set (system-level + derivative-scoped, as applicable)
5. Evidence: tests, traces, audits, or validation outputs

This repository does not mandate _how_ proof is produced, only that proof is possible.

---

## Forks and Copies

Forking this repository does not move canonical authority.

- Forks are **non-canonical by definition**.
- Forks may be useful, even superior for local purposes.
- Canonical meaning remains with the canonical repository and its `canon/INDEX.md`.

Disagreement does not invalidate authority.
Silence does not weaken authority.
Ambiguity is resolved by Canon, not by social process.

---

## Change Control (Pointer)

Change control mechanics are defined in:

- `FREEZE.md`
- `IMMUTABILITY.md`
- `RELEASE.md`
- `versions/`

This file defines **authority boundaries**; change control defines **how and when** canonical artifacts may change.
