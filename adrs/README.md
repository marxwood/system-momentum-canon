# Architectural Decision Records (ADRs)

This directory contains **system-level ADRs**.

These ADRs:

- apply across multiple derivatives,
- define architectural decisions with long-term impact,
- are normative but non-canonical,
- must explicitly reference the Canon.

This directory does **not** contain:

- derivative-scoped ADRs (those live inside `/derivatives/*/adrs/`),
- implementation decisions,
- technology selections.

---

## Authority Level

System-level ADRs operate at **Authority Level 3**  
(see `governance/authority.md`).

They:

- MUST comply with Canon,
- MUST NOT introduce new canonical concepts,
- MUST NOT redefine Canon terminology.

---

## Scope Rules

A system-level ADR may:

- select or reject architectural perspectives,
- define global constraints or invariants,
- standardize cross-derivative practices.

A system-level ADR must NOT:

- specify runtime architecture,
- specify programming languages,
- specify infrastructure or vendors,
- describe implementation details.

---

## Required References

Each ADR MUST include:

- Canon reference(s) (section or document),
- Scope statement (what it applies to),
- Explicitly rejected alternatives.

---

## Numbering

ADR numbering is local to this directory.

There is **no ADR-0 here**.

ADR-0 is conceptually equivalent to the Canon itself  
(see `governance/authority.md`).

---

## Status

Each ADR MUST declare a status:

- Proposed
- Accepted
- Deprecated
- Superseded
