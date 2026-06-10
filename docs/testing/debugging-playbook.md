# Debugging Playbook

1. Reproduce the request with the smallest scenario target.
2. Inspect sanitized payload from `_build_scenario_payload`.
3. Check graph lookup params before debugging Neo4j.
4. Force graph failure to verify fallback behavior.
5. Run focused Django test classes before the full core suite.
6. For ingestion failures, decode the Pub/Sub envelope and validate the embedded JSON first.
