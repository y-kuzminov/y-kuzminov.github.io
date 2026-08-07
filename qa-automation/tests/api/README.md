# API Autotests

pytest + requests against a public REST API (jsonplaceholder.typicode.com / reqres.in).

**Covered:**
- GET (list / single resource)
- POST (create)
- 404 handling
- Nested resources
- Basic assertions on status code and response body

**Run:**
```bash
pytest tests/api -v
