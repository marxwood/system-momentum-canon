# Projection Constraints

This document defines **structural constraints** for projections.
All constraints **derive from Core projection invariants** and do not introduce new rules.

No constraint in this document grants authority, behavior, or governance.

---

## Constraint Classes

### 1. Scope Separation

Projections of different scopes are structurally non-substitutable.

- `public` ≠ `operational`
- `operational` ≠ `analytical`
- `analytical` ≠ `governance`

Cross-scope substitution constitutes a structural violation.

---

### 2. Authority Isolation

No projection may acquire authority outside its declared scope.

- Projections do not decide
- Projections do not govern
- Projections do not commit
- Projections do not redefine system meaning

Authority remains external to projections.

---

### 3. Directionality

All projections are unidirectional.

- State → Projection is permitted
- Projection → State is prohibited

Any reverse coupling is a violation.

---

### 4. Intent Preservation

Projection intent must remain stable across usage.

- `display` projections may not coordinate or inspect
- `coordination` projections may not decide or commit
- `inspection` projections may not influence execution

Intent mutation constitutes projection drift.

---

### 5. Temporal Integrity

Temporal mode may not be altered implicitly.

- `snapshot` may not behave as `live`
- `live` may not retroactively modify history
- `historical` may not project current authority

Temporal leakage is a structural fault.

---

This document introduces no additional semantics.
