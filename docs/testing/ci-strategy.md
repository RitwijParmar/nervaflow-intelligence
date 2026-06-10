# CI Strategy

Recommended jobs:

- `django-core`: install Python dependencies and run `python manage.py test aetherchain.core`.
- `static-sanity`: check import safety for optional GCP and graph integrations.
- `docs-links`: verify STLC docs remain present for release review.

Keep CI deterministic by mocking Neo4j, GCP tokens, and external discovery APIs.
