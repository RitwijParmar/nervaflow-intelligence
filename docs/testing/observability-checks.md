# Observability Checks

During testing, inspect:

- Response status and structured fields for simulation endpoints.
- Raw context flags that identify narrative source and impacted asset counts.
- Logs for graph fallback warnings.
- Pub/Sub worker responses: 204 for accepted events and 500 for rejected processing.

For failed simulations, capture the event payload after sanitation.
