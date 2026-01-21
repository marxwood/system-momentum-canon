# Brain — Canonical Functional Domains

This document describes the internal functional structure of the Brain
as a canonical derivative of the System Momentum Canon.

The domains defined here specify **what functional capacities must exist**
for the Brain to enact the Canon, without defining implementation,
control flow, or usage patterns.

---

## 1. Perceptual Domain

### Purpose

Intake and structuring of incoming signals into **percepts**.

### Inputs

- world signals (external observations)
- system signals (internal state observations)
- user-provided inputs

### Outputs

- percepts (structured candidates)
- provenance anchors (source, time, channel)
- optional signal quality indicators

### Boundary Conditions

- Produces candidates only.
- Assigns no meaning.
- Asserts no truth.
- Creates no memory.

### Non-Responsibilities

- semantic interpretation
- reasoning or inference
- validation or evaluation
- persistence
- action

### Interfaces

- feeds percepts into the Cognitive / Reasoning Domain

---

## 2. Cognitive / Reasoning Domain

### Purpose

Ephemeral reasoning over percepts to produce structured candidates
for interpretation, evaluation, or action.

### Characteristics

- transient
- non-persistent
- non-authoritative

### Inputs

- percepts from the Perceptual Domain
- semantic context references (read-only)

### Outputs

- structured hypotheses
- candidate interpretations
- candidate actions
- intermediate reasoning artifacts

### Boundary Conditions

- Produces no commitments.
- Produces no institutional memory.
- Produces no semantic authority.

### Non-Responsibilities

- defining meaning
- asserting validity
- storing results
- executing actions

### Interfaces

- consults Knowledge / Semantic Authority Domain
- passes candidates to Reflective or Action / Governance Domain

---

## 3. Knowledge / Semantic Authority Domain (KSA)

### Purpose

Maintain **authoritative semantic meaning** within the system.

### Responsibilities

- definition of terms
- semantic constraints
- conceptual consistency
- canonical interpretation boundaries

### Inputs

- semantic definitions
- controlled updates via governance

### Outputs

- authoritative meaning references
- semantic constraints applied system-wide

### Boundary Conditions

- Does not store events or decisions.
- Does not perform reasoning.
- Does not create claims.

### Non-Responsibilities

- perception
- inference
- memory of occurrences
- action

### Interfaces

- consulted by Cognitive, Reflective, and Action domains
- constrained by Core Authority rules

---

## 4. Institutional / Epistemic Memory Domain (IEM)

### Purpose

Canonical persistence of **claims, decisions, states, and validity**.

### Responsibilities

- store what the system is institutionally committed to
- maintain auditability and temporal continuity
- anchor responsibility and accountability

### Inputs

- validated claims
- authorized decisions
- governance outcomes

### Outputs

- canonical memory objects
- historical record
- responsibility traces

### Boundary Conditions

- Only authorized inputs may enter.
- Immutable once committed (except via governance).

### Non-Responsibilities

- perception
- reasoning
- semantic definition
- action initiation

### Interfaces

- feeds Reflective Domain
- consulted by Action / Governance Domain

---

## 5. Reflective Domain

### Purpose

System self-observation and critique.

### Responsibilities

- examine past decisions and claims
- detect inconsistencies, drift, or failure modes
- generate heuristics and meta-insights

### Inputs

- institutional memory from IEM
- analytical projections

### Outputs

- critique signals
- heuristic proposals
- governance-relevant insights

### Boundary Conditions

- Produces no authority.
- Produces no direct action.
- Produces no canonical memory.

### Non-Responsibilities

- enforcement
- execution
- semantic redefinition

### Interfaces

- informs Action / Governance Domain
- depends on IEM for grounding

---

## 6. Action / Governance Domain

### Purpose

Authorize and enact **state-changing decisions**.

### Responsibilities

- evaluate candidates for action
- apply governance rules
- commit decisions into IEM

### Inputs

- candidate actions from Cognitive Domain
- semantic constraints from KSA
- historical context from IEM
- reflective signals from Reflective Domain

### Outputs

- authorized decisions
- committed state changes

### Boundary Conditions

- Only domain allowed to create commitments.
- All actions are accountable and auditable.

### Non-Responsibilities

- perception
- reasoning
- semantic definition

### Interfaces

- writes to Institutional / Epistemic Memory
- constrained by Core Authority and Regimes

---

## Closure Rule

The set of Canonical Functional Domains is **closed**.

No domain may be added, removed, merged, or reinterpreted
without an explicit Canon amendment.
