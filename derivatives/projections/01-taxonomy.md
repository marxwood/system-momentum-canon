# Projection Taxonomy

This document defines the **structural classification axes** for projections.
It introduces no behavior, authority, or operational rules.

---

## Axes

### 1. Scope

Defines the exposure and audience boundary of the projection.

- `public`
- `operational`
- `analytical`

---

### 2. Intent

Defines the primary structural purpose of the projection.

- `display` — presentation of already-established state
- `coordination` — alignment of ongoing system activity
- `inspection` — examination of system state without effect

---

### 3. Temporal Mode

Defines the time relationship of the projection to underlying state.

- `snapshot` — point-in-time representation
- `live` — continuously updating representation
- `historical` — past-state representation

---

### 4. Coupling

Defines the structural dependency between the projection and the system.

- `loose` — read-only, non-binding
- `bound` — directly reflects active system state
- `authoritative` — defines canonical operational surface

---

### 5. Stability

Defines the persistence characteristics of the projection.

- `ephemeral` — transient, non-retained
- `persistent` — retained across sessions
