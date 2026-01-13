# Product Requirement Documents (PRDs)

This directory contains **system-level PRDs**.

PRDs define **normative realization expectations**:
what must be true if a system claims to implement
a Canon-compliant derivative.

PRDs:

- do NOT describe implementation,
- do NOT describe architecture,
- do NOT select technology,
- define conditions of correctness.

---

## Authority Level

System-level PRDs operate at **Authority Level 3**  
(see `governance/authority.md`).

They:

- MUST comply with Canon,
- MAY reference derivatives for scope,
- MUST remain implementation-agnostic.

---

## Scope Rules

A system-level PRD may:

- define required capabilities,
- define required behaviors,
- define observable properties,
- define failure expectations.

A system-level PRD must NOT:

- describe system internals,
- reference code modules,
- prescribe data structures,
- include deployment assumptions.

---

## Required References

Each PRD MUST include:

- Canon reference(s),
- Capability or obligation description,
- Explicit non-requirements.

---

## Status

Each PRD MUST declare a status:

- Draft
- Active
- Deprecated
- Superseded
