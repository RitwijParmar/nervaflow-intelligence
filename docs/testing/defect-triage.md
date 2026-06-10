# Defect Triage

## Severity

- S0: authenticated endpoint bypass, worker crash loop, or scenario response corruption.
- S1: incorrect impacted assets, broken fallback, malformed catalog response, or ingestion data loss.
- S2: weak discovery text, missing evidence snippet, or UI copy mismatch.

## Required Evidence

Record request JSON, auth header state, graph query params, mocked external dependency response, and whether fallback logic was used.
