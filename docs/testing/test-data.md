# Test Data

Scenario targets:

- Location: `Port of Los Angeles`
- Supplier: `Acme Components`
- SKU list: `SKU-1, sku-1, SKU-2`
- Route list: `R-1`

Boundary values:

- Empty request should return a validation error.
- Long `context_note` should be trimmed to 280 characters.
- `horizon_days=999` should clamp to 180.
- Duplicate SKUs should deduplicate case-insensitively.
