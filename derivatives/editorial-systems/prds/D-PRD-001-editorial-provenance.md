# D-PRD-001: Provenance Visibility in Editorial Artifacts

## Status

Active

## Purpose

Ensure that all editorial artifacts expose the provenance
of claims, interpretations, and assertions.

## Canon References

- Canon: Truth requires provenance
- Canon: Uncertainty must not be hidden
- ADR-0: Interpretation and observation are distinct

## Derivative Scope

This PRD applies only to: `derivatives/editorial-systems`.

## Requirements

- Editorial artifacts MUST expose the source of each factual claim.
- Interpretations MUST be labeled as such.
- Absence of sufficient provenance MUST be observable.
- Contradictory claims MAY coexist without forced resolution.

## Non-Requirements

- No requirement for a specific citation format.
- No requirement for automated fact validation.
- No requirement for real-time verification.

## Validation

Compliance can be validated by inspecting editorial artifacts
for explicit provenance and interpretive markers.

## Notes

This PRD defines correctness conditions, not editorial workflow.
