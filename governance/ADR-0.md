# ADR-0 — Constitutional Architecture (Explainer)

This document is an **explanatory artifact**.

It is **not** an Architectural Decision Record in the procedural sense.
It has no status, no lifecycle, and cannot be superseded.

Its sole purpose is to **make explicit the constitutional constraints
that are already implied by the System Momentum Canon**.

---

## What ADR-0 Is

ADR-0 represents the **constitutional architecture** of the system.

It is the Canon:

- translated into non-negotiable architectural constraints,
- expressed in enforceable form,
- without introducing new meaning.

ADR-0 does **not** add to the Canon.
It **derives from it**.

---

## What ADR-0 Is Not

ADR-0 is not:

- a design decision,
- an implementation choice,
- a technology selection,
- a runtime optimization,
- an ADR that can be accepted, rejected, or superseded.

ADR-0 is **outside the ADR mechanism**.

---

## Relationship to the Canon

The relationship is strictly one-way:

System Momentum Canon
↓ (derivation, not interpretation)
ADR-0 — Constitutional Architecture

- Canon defines **what is true**.
- ADR-0 defines **what must never be violated** in architecture or execution.

Canon remains the source of meaning.
ADR-0 is the source of **absolute constraints**.

---

## Core Constitutional Constraints

The following constraints are **binding** for all derivatives,
all ADRs, all PRDs, and all implementations.

1. **Canonical authority is singular**  
   There is exactly one Canon. No architectural layer may override it.

2. **No implicit authority exists**  
   All authority must be explicit, scoped, and auditable.

3. **Responsibility is non-delegable**  
   Accountability cannot be transferred to agents, automation, or abstraction layers.

4. **Truth is never inferred without provenance**  
   All truth claims must be traceable to observations, context, and time.

5. **Interpretation and observation are distinct**  
   The system must never collapse interpretation into fact.

6. **Contradiction is representable**  
   The system must allow mutually incompatible truths to coexist without forced resolution.

7. **Resolution is explicit**  
   Any reconciliation of contradiction must be a deliberate, auditable action.

8. **Auditability is mandatory**  
   Actions, decisions, and state transitions must be observable and reviewable.

9. **History is append-only**  
   Past states may not be erased or overwritten without trace.

10. **Forgetting is intentional**  
    Loss of memory must be explicit, justified, and bounded.

11. **Uncertainty must not be hidden**  
    The system must preserve and expose uncertainty where it exists.

12. **Silence is a valid system state**  
    The system must be allowed to withhold action or output when constraints are unmet.

13. **No execution outside declared capability**  
    Actions may occur only within explicitly granted capabilities.

14. **Scale must not erase meaning**  
    Architectural shortcuts that degrade meaning for efficiency are prohibited.

15. **All lower layers are subordinate**  
    Derivatives, ADRs, PRDs, agents, and implementations must comply with these constraints.

---

## Enforcement Scope

These constraints apply to:

- all derivatives,
- all system-level ADRs and PRDs,
- all derivative-scoped ADRs and PRDs,
- all implementation repositories,
- all human and machine agents operating under System Momentum.

Violation of ADR-0 is, by definition, a violation of the Canon.

---

## Change Policy

ADR-0 cannot be changed directly.

Any change to these constraints can occur **only** by:

- revising the Canon itself,
- following the Canon revision and governance process.

If the Canon changes, ADR-0 changes implicitly.

---

## Why This Document Exists

ADR-0 is documented here to:

- prevent misinterpretation of Canon authority,
- provide a clear enforcement reference for builders,
- eliminate ambiguity during implementation pressure,
- close the gap between epistemology and architecture.

This document introduces **no new rules**.
It only makes existing ones unavoidable.

---

## Final Statement

ADR-0 is not optional.
ADR-0 is not negotiable.
ADR-0 is not an architectural preference.

ADR-0 is the **constitutional boundary of the system**.
