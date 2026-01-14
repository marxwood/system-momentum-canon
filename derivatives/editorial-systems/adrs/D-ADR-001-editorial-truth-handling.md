# D-ADR-001: Explicit Separation of Observation and Interpretation

## Status

Accepted

## Context

Editorial systems operate in environments where statements, events,
and interpretations are frequently conflated.

Without explicit separation, editorial output risks collapsing
interpretation into fact, violating Canon truth constraints.

## Decision

Editorial systems MUST explicitly distinguish:

- observed statements or events,
- editorial interpretation or analysis.

No editorial artifact may present interpretation as observation.

## Canon References

- Canon: Truth is contextual and temporal
- Canon: Observation and interpretation are distinct
- ADR-0: Truth is never inferred without provenance

## Derivative Scope

This ADR applies only to: `derivatives/editorial-systems`.

## Consequences

- Editorial artifacts require explicit provenance markers.
- Interpretive layers must be identifiable and auditable.
- Ambiguity may persist without forced resolution.

## Rejected Alternatives

- Implicit interpretation based on source authority (rejected: violates non-delegable responsibility).
- Automated truth inference without provenance (rejected: violates Canon truth model).

## Non-Goals

- Defining UI representation.
- Defining storage models.
- Defining agent implementation.

## Notes

This ADR constrains meaning, not format.
