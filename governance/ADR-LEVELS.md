# ADR Levels and Authority Boundaries

This document defines **all ADR levels** used across the System Momentum ecosystem
and explicitly states **where each level may exist**.

This is a governance artifact.
It does not introduce new rules.
It formalizes existing boundaries.

---

## Purpose

The purpose of this document is to:

- prevent category errors between truth, obligation, and execution,
- avoid architectural drift caused by misplaced ADRs,
- make audit boundaries explicit,
- ensure long-term system coherence.

---

## ADR Levels Overview

ADR levels are hierarchical.
Higher levels constrain lower levels.
Lower levels must never influence higher levels.

Level 0 — Canon
Level 0.5 — ADR-0 (Constitutional Architecture)
Level 3 — System-level ADRs
Level 4 — Derivative-scoped ADRs
Level 5 — Implementation ADRs

Levels 1 and 2 are intentionally unused to avoid false granularity.

---

## Level 0 — Canon

**Location**

- `/canon`

**Nature**

- Ontological and epistemological truth.
- Defines what is true about the system.

**Properties**

- Immutable by default.
- Changes only via Canon revision process.
- Never references lower layers.

**Examples**

- Truth is contextual and temporal.
- Responsibility is non-delegable.
- Uncertainty must not be hidden.

---

## Level 0.5 — ADR-0 (Constitutional Architecture)

**Location**

- Implicit in Canon
- Explicitly documented as: `/governance/ADR-0.md`

**Nature**

- Canon translated into non-negotiable architectural constraints.

**Properties**

- Derived, not decided.
- Outside ADR lifecycle.
- Cannot be superseded.

**Function**

- Defines what must never be violated by architecture or execution.

---

## Level 3 — System-level ADRs

**Location**

- `/adrs`

**Nature**

- Cross-derivative architectural decisions.

**Properties**

- Normative, non-canonical.
- Small in number.
- Long-lived.

**Scope**

- Apply to multiple derivatives.
- Standardize system-wide constraints.

**Restrictions**

- Must not introduce new canonical concepts.
- Must not specify implementation details.

---

## Level 4 — Derivative-scoped ADRs

**Location**

- `/derivatives/<derivative-name>/adrs`
- Naming convention: `D-ADR-XXX`

**Nature**

- Context-specific architectural decisions.

**Properties**

- Numerous.
- Scoped to a single derivative.
- Canon- and ADR-0-compliant.

**Scope**

- Resolve tensions specific to one realization context
  (editorial, agentic, institutional, etc.).

---

## Level 5 — Implementation ADRs

**Location**

- **External implementation repositories only**

**Nature**

- Engineering and execution decisions.

**Examples**

- Technology selection
- Data storage strategy
- Deployment topology
- Performance optimizations

**Properties**

- Highly specific
- Shorter-lived
- Replaceable

---

## Explicit Prohibition

**Level 5 ADRs MUST NOT exist in this repository.**

This repository is authoritative for:

- truth,
- constraints,
- obligations.

It is NOT authoritative for:

- execution,
- tooling,
- infrastructure.

Any ADR that:

- mentions specific technologies,
- discusses deployment,
- optimizes performance,
- selects vendors or platforms

**does not belong here and must be moved to an implementation repository.**

---

## Dependency Rules

- Level 5 ADRs MUST reference:

  - Canon version
  - Relevant derivative
  - Applicable Level 3 and Level 4 ADRs

- Level 4 ADRs MUST reference:

  - Canon
  - ADR-0
  - (optionally) system-level ADRs

- Level 3 ADRs MUST reference:
  - Canon

No level may reference a lower one as a source of authority.

---

## Audit Implications

If an architectural question arises:

- Ask first: _which ADR level does this belong to?_
- If the answer is unclear, default upward.

Misplaced ADRs are a **structural defect**, not a documentation issue.

---

## Final Rule

The closer a decision is to execution,
the more ADRs will exist,
but the less authority they carry.

This hierarchy is mandatory.
