# Operational System State (OSS) Surface

This document defines the **Operational System State (OSS)** as an
**interactive operational projection surface**.

The OSS surface exists to expose the current operational state
of the system as a whole, in a form suitable for monitoring,
coordination, and governance oversight.

It is a visibility surface, not a control plane.

---

## 1. Purpose

The OSS surface exists to:

- provide a coherent snapshot of system-wide operational state
- surface health, load, and status indicators
- support oversight and coordination
- enable timely detection of anomalies

The OSS surface does **not** authorize actions or decisions.

---

## 2. Canonical Dependencies

This surface depends on:

- **Core / Projections**  
  (permission for system-wide state projections)

- **Derivatives / Projections**  
  (constraints on operational aggregation)

- **Brain**  
  (canonical objects representing state, actions, and outcomes)

All rendered state is derived, scoped, and constrained.

---

## 3. Visible Elements

The OSS surface may render:

- global status indicators
- subsystem health summaries
- active regimes or constraints
- throughput or load signals
- error rates or failure markers
- temporal state snapshots

Elements represent **state**, not intent or command.

---

## 4. Permitted Interactions

Depending on governance and role, the surface may allow:

- filtering and slicing of state views
- navigation to related operational surfaces
- acknowledgment of alerts
- annotation for audit or review

No direct execution or mutation is permitted from OSS.

---

## 5. Constraints

The OSS surface must enforce:

- read-only defaults
- strict separation between visibility and control
- regime-based access limits
- clear distinction between observation and intervention

The surface must never:

- imply urgency as obligation
- collapse state into instruction
- expose hidden authority
- act as a control surface

---

## 6. People and Agents

Both people and agents may observe OSS.

Agents may:

- monitor system state
- detect anomalies
- generate alerts or reports

Agents may **not**:

- initiate actions directly
- infer permission from visibility
- bypass governance using OSS signals

---

## 7. Non-Equivalence Rules

- OSS ≠ control plane
- OSS ≠ command interface
- OSS ≠ authority
- OSS ≠ decision engine

The OSS is a **system-wide visibility surface**, nothing else.

---

## 8. Scope Discipline

This document defines:

- what system state may be surfaced
- how it may be observed
- what constraints apply

Narrative explanation belongs to **Doctrines**.  
Canonical rules belong to **Core**.  
Structural models belong to **Derivatives**.
