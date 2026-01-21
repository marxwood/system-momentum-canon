# Operational Dashboard Surface

This document defines the **Operational Dashboard** as an
**interactive operational projection surface**.

The dashboard is a situational awareness surface.
It exists to summarize system state and surface signals
relevant for coordination and decision-making,
without asserting authority or truth.

---

## 1. Purpose

The Operational Dashboard exists to:

- provide a consolidated view of operational state
- surface alerts, statuses, and indicators
- support coordination across actions and actors
- reduce cognitive load during operation

The dashboard does **not** decide, evaluate, or authorize actions.

---

## 2. Canonical Dependencies

This surface depends on:

- **Core / Projections**  
  (permission for operational state projections)

- **Derivatives / Projections**  
  (classification and constraints of operational views)

- **Brain**  
  (canonical objects representing state, actions, and signals)

No dashboard element has independent authority.

---

## 3. Visible Elements

The dashboard may render:

- status indicators
- alerts and warnings
- progress summaries
- queues or backlogs
- linked canonical objects
- temporal snapshots

All elements are **derived views**, not canonical facts by themselves.

---

## 4. Permitted Interactions

Depending on governance and role, the surface may allow:

- filtering and grouping
- acknowledgment of alerts
- navigation to related surfaces
- proposal of follow-up actions
- annotation or tagging (non-authoritative)

Any action beyond acknowledgment or navigation
requires upstream authorization.

---

## 5. Constraints

The dashboard surface must enforce:

- read-only defaults for state representation
- regime-based access control
- separation between signal and decision
- clear distinction between alert and mandate

The surface must never:

- imply obligation
- fabricate urgency
- override governance
- collapse signal into command

---

## 6. People and Agents

Both people and agents may use the dashboard.

Agents may:

- monitor indicators
- raise alerts
- suggest actions

Agents may **not**:

- escalate state into authority
- infer permission from visibility
- execute actions directly from the dashboard

---

## 7. Non-Equivalence Rules

- Dashboard ≠ command center
- Dashboard ≠ authority
- Dashboard ≠ decision engine
- Dashboard ≠ ground truth

The dashboard is a **situational awareness surface**, nothing else.

---

## 8. Scope Discipline

This document defines:

- what is surfaced
- how it may be interacted with
- what constraints apply

Narrative explanation belongs to **Doctrines**.  
Canonical rules belong to **Core**.  
Structural models belong to **Derivatives**.
