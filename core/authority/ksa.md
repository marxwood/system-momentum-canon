# Knowledge / Semantic Authority (KSA)

KSA defines the canonical authority layer responsible for **meaning**.

KSA is not a runtime, not an agent, and not an implementation.  
KSA is a **normative discipline**: it determines who may define terms, how terms are anchored, and how semantic changes propagate through the Canon.

---

## 1. Purpose

KSA exists to prevent semantic collapse.

Without KSA, systems drift into:

- shifting definitions
- policy disguised as meaning
- retroactive reinterpretation
- claims that cannot be evaluated because terms are unstable

KSA answers:

> Who is allowed to define meaning, under which constraints, and with what accountability?

---

## 2. Scope

KSA governs:

- terms, definitions, and controlled vocabularies
- semantic boundaries between concepts
- permissible transformations of definitions
- semantic compatibility across versions

KSA does **not** govern:

- truth
- decisions
- execution
- operational workflows
- UI and projections

---

## 3. Authority Objects

KSA manages canonical semantic objects:

- **Term**: a named concept with a stable identifier
- **Definition**: the canonical meaning of a term
- **Boundary**: constraints separating adjacent terms (what a term is _not_)
- **Mapping**: allowable equivalences or translations between terms/contexts
- **Change**: a semantically accountable modification to any of the above

These objects are canonical artifacts. Implementations may store them in any form, but cannot alter their meaning outside KSA rules.

---

## 4. Semantic Stability Guarantees

KSA provides stability guarantees:

1. **Referential stability**  
   A term must remain referable across time and contexts.

2. **Interpretive constraints**  
   Definitions are constrained by boundaries and by Canon-level invariants.

3. **Change accountability**  
   Semantic changes must be explicitly authored, justified, and versioned.

4. **Non-retroactivity by default**  
   A semantic change does not silently rewrite the meaning of past claims.

---

## 5. Relationship to Core Constitution

The Constitution defines **what must be protected**.  
KSA defines **how meaning is protected**.

The Constitution can forbid classes of semantic behavior (e.g., semantic drift), while KSA defines the operational semantics of enforcing those prohibitions (as canonical rules, not runtime operations).

---

## 6. Relationship to Validity

Validity evaluates **claims**, but claims are only evaluable if their terms are stable.

Therefore:

- Validity is downstream of KSA.
- KSA failure implies validity collapse.

---

## 7. Relationship to Derivatives and Doctrines

Derivatives and doctrines may introduce:

- new capabilities
- new practices
- new projections

They may not introduce new meaning outside KSA.

A doctrine can propose interpretation practices; it cannot redefine definitions.

---

## 8. Non-Equivalence Rules

- KSA ≠ “intelligence”
- KSA ≠ “truth authority”
- KSA ≠ “policy engine”
- KSA ≠ “ontology implementation”
- KSA ≠ “editorial guidelines”

KSA is semantic authority, not operational authority.

---

## 9. Minimal KSA Invariants

The following invariants are core:

- **Explicit authorship** of semantic change
- **Versioned semantics** (terms and definitions are version-addressable)
- **Traceable propagation** (downstream artifacts can declare which semantic version they use)
- **Non-silent reinterpretation** (past claims keep their semantic context)
