# Test Matrix

| Area | Test Type | Coverage Target | Priority |
| --- | --- | --- | --- |
| Scenario API | DRF integration | auth, public access, validation, structured response | P0 |
| Input cleaning | Unit | text trim, list dedupe, horizon clamp, default event type | P0 |
| Pub/Sub worker | Integration/unit | valid envelope, missing data, malformed payload | P0 |
| Graph lookup | Unit | location, supplier, SKU-only, route-only query shape | P0 |
| Graph fallback | Integration | Neo4j failure returns useful simulated assets | P0 |
| Catalog options | API/unit | kind validation, filtering, fallback catalog | P1 |
| Retrieval evidence | Unit | supporting snippets and score shape | P1 |
| GDELT ingestion | Unit | query normalization, discovery documents, date parsing | P1 |
