# Content Stratification Rules

This document defines **mandatory rules for content placement**
within the System Momentum Canon repository.

Its purpose is to prevent:

- conceptual duplication across layers
- narrative leakage into canonical documents
- erosion of the Canon / Derivatives / Doctrines distinction

These rules are binding.

---

## 1. Canon (core/)

### Purpose

Canon defines **what must be true** for a system to be canonical.

### Canon MUST:

- state invariants
- define boundaries
- establish prohibitions
- remain minimal and closed

### Canon MUST NOT:

- explain why something matters
- include examples
- include historical context
- describe failure modes
- discuss trade-offs
- teach or persuade
- include human-oriented narrative

If a sentence can be removed without breaking canonical validity,
it does not belong in Canon.

---

## 2. Derivatives (derivatives/)

### Purpose

Derivatives define **structural decompositions**
of already-established canonical truths.

### Derivatives MUST:

- enumerate types, categories, or domains
- define relations between elements
- provide maps of the conceptual space

### Derivatives MUST NOT:

- justify why a structure exists
- warn about misuse
- describe consequences
- include narrative or examples
- repeat canonical definitions verbatim

Derivatives answer **“how the space is structured”**, not “why”.

---

## 3. Doctrines (doctrines/)

### Purpose

Doctrines exist to make the Canon **intelligible to humans**.

They explain consequences, risks, power dynamics,
and historical failure modes.

### Doctrines MUST:

- explain _why_ structures matter
- describe systemic risks and collapse modes
- include trade-offs and tensions
- connect abstract rules to real-world behavior
- be readable as essays

### Doctrines MUST NOT:

- redefine canonical rules
- introduce new authority
- contradict Canon
- be reduced to bullet lists only

If a doctrinal text could be mechanically summarized
without losing meaning, it is insufficient.

---

## 4. Duplication Prohibition Rule

No concept may appear with the **same explanatory content**
in more than one layer.

Allowed duplication:

- naming
- references
- pointers

Forbidden duplication:

- re-explaining the same idea
- paraphrasing instead of relocating content
- “progressive expansion” of the same text across layers

When duplication occurs, content must be **removed from the higher layer**
and relocated downward.

---

## 5. Escalation Rule

If during writing it becomes necessary to:

- explain consequences
- justify a design choice
- warn about misuse
- discuss power, politics, or society

The content MUST be moved to Doctrine.

Escalation upward (Doctrine → Derivative → Canon) is forbidden.

---

## 6. Reader Contract

Each layer assumes a different reader:

- Canon assumes a **validator**
- Derivatives assume a **system designer**
- Doctrines assume a **human operator or thinker**

Writing must respect the assumed reader.
Violation of reader contract is a structural error.

---

## 7. Enforcement

Content violating these rules is considered:

- non-canonical
- non-binding
- subject to removal or relocation

No exception is permitted without explicit governance amendment.
