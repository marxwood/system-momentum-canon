# Canon Immutability Notice

This document defines the **immutability guarantees** of released versions of the System Momentum Core Canon.

This document is **non-canonical**.
It introduces no meaning and confers no authority.

---

## Immutable Releases

All tagged releases of the Core Canon are **immutable**.

Immutability means:

- no force-pushes
- no tag movement
- no history rewriting
- no retroactive changes

Once published, a release is permanent.

---

## Scope of Immutability

Immutability applies to:

- release tags (e.g. `v0.1`)
- commit history referenced by those tags
- canonical documents under `canon/` at the time of release
- associated status and audit records

---

## Corrections and Revisions

If errors are discovered after a release:

- a **new version** must be created
- the prior release remains unchanged
- corrections are documented, not overwritten

There is no retroactive correction.

---

## No Silent Updates

Silent updates are prohibited.

Any change affecting canonical meaning must:

- be explicit
- be versioned
- be auditable

Silence must not be used to mask change.

---

## Relationship to Governance

Immutability is enforced by repository practice and governance policy.

It does not:

- alter canonical meaning
- grant authority
- replace change procedures

---

## Status

Immutability active for all released versions.
