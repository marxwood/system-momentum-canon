# Validity

Validity is the canonical discipline for evaluating **claims**.

Validity is not truth.  
Validity is not belief.  
Validity is not decision.

Validity answers:

> Under which regime, with which evidence, and under which interpretation constraints is a claim admissible and maintainable?

---

## 1. Claim Model

A claim minimally contains:

- **Statement**: what is being asserted
- **Provenance**: origin and chain of custody
- **Semantic context**: which KSA version(s) define the terms used
- **Regime context**: which regime governs evaluation
- **Support set**: evidence and supporting claims
- **Contradiction set**: direct conflicts, counter-evidence, rival claims
- **Status**: admitted / contested / invalidated / retired

Claims are canonical objects; implementations may store them differently but must preserve these conceptual fields.

---

## 2. Admission

Admission means: the claim is allowed to exist inside the system as a first-class object.

Admission requires:

- a declared regime
- a declared semantic context (KSA)
- minimal provenance

Admission does not require the claim to be “true”.

---

## 3. Evaluation

Evaluation produces regime-specific validity outcomes.

A claim may be:

- **maintained** (still admissible under current evidence)
- **contested** (admissible but under active contradiction)
- **invalidated** (no longer admissible under regime rules)
- **retired** (superseded or deprecated, without implying falsity)

---

## 4. Invalidation

Invalidation is a regime-governed event.

Typical invalidation triggers:

- provenance failure (fabrication, broken chain, unknown origin)
- semantic mismatch (terms not grounded in declared KSA context)
- regime rule violation (insufficient evidence class, inadmissible claim class)
- decisive contradiction under regime rules

Invalidation is not deletion.  
An invalidated claim remains referable, with its invalidation trail.

---

## 5. Temporal Discipline

Claims carry time in two ways:

- time of assertion
- time of evaluation

A claim valid at time T under regime R may become contested or invalidated later without retroactively rewriting historical context.

---

## 6. Relationship to Projections

Projections must treat validity as contextual.

A projection may present:

- “valid under regime X”
- “contested”
- “invalidated”

A projection must not present:

- regime-less “truth”
- implied certainty without provenance and context

---

## 7. Minimal Validity Invariants

- Every claim must declare semantic context (KSA) and regime.
- Admission requires minimal provenance.
- Invalidation preserves trails and referability.
- Validity outcomes are regime-scoped, not universal.
