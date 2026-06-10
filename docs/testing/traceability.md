# Traceability

| Requirement | Code Surface | Test Surface |
| --- | --- | --- |
| Require at least one scenario target | `core.views._build_scenario_payload` | `SimulateImpactTests`, `PublicExperienceTests` |
| Accept SKU and route scoped simulations | `core.views`, `core.tasks._build_graph_lookup` | `PublicExperienceTests`, graph lookup tests |
| Decode Cloud Pub/Sub envelopes | `core.views._decode_pubsub_envelope` | `WorkerIngressTests`, sanitization tests |
| Fallback when Neo4j is unavailable | `core.tasks.run_impact_analysis` | `SimulateImpactTests` |
| Normalize graph result rows | `core.tasks._normalize_graph_rows` | `ScenarioInputSanitizationTests` |
| Enforce API token on alerts | `core.permissions.IsBearerAuthenticated` | `SimulateImpactTests` |
