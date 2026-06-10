# Regression Suite

Run core tests from the Django source folder:

```bash
cd src
python manage.py test aetherchain.core
```

For focused debugging:

```bash
cd src
python manage.py test aetherchain.core.tests.ScenarioInputSanitizationTests
python manage.py test aetherchain.core.tests.SimulateImpactTests
```

Mock Neo4j, GCP, and external HTTP calls unless the test is explicitly marked as an integration smoke check.
