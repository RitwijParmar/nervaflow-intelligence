# Security Checks

Verify:

- `alert-list` requires `Bearer` auth.
- Public simulation remains unauthenticated by design but still validates targets.
- Worker ingestion accepts only POST.
- Input strings are stripped and length-limited before graph lookup.
- Future write endpoints include explicit authorization tests.
