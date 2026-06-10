# STLC Plan

## Scope

Validate scenario simulation, public and authenticated API behavior, Pub/Sub worker ingestion, catalog lookup, graph fallback, evidence retrieval, and GDELT discovery ingestion.

## Phases

1. Requirement analysis: confirm target inputs, API auth, catalog filters, and fallback behavior.
2. Test planning: prioritize input sanitization, graph query construction, fallback quality, and ingestion resilience.
3. Test design: combine Django API tests, helper unit tests, and mocked external dependency tests.
4. Environment setup: run Django tests with mocked Neo4j, GCP, retrieval, and HTTP calls.
5. Execution: run focused core tests before PR review and full suite before release.
6. Closure: every production defect should add a regression test in `src/aetherchain/core/tests.py`.

## Exit Criteria

- Scenario payload tests cover missing targets, SKU/route scope, text trimming, and horizon bounds.
- Worker ingestion rejects malformed Pub/Sub envelopes.
- Graph fallback behavior remains deterministic when Neo4j is unavailable.
