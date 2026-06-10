# Release Gates

Do not release if:

- Protected alert APIs can be read without a valid token.
- Scenario simulation accepts empty targets.
- Graph fallback returns no useful impacted assets for valid scenarios.
- Pub/Sub worker cannot process a valid envelope.
- Catalog kind validation breaks supported values.
