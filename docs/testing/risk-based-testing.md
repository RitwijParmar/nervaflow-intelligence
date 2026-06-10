# Risk-Based Testing

Highest risk areas:

- Scenario input sanitation because user-entered targets drive graph queries.
- Pub/Sub envelope parsing because malformed events can cause worker retries.
- Graph fallback because demos and degraded environments depend on useful output.
- API authorization because alert data is protected while public simulation is intentionally open.

Lower risk areas:

- Static homepage content.
- Documentation-only catalog examples.
