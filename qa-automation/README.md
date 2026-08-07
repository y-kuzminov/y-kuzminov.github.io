# Automation

Test automation practice with Python.

### Stack
- **API:** pytest + requests
- **UI:** pytest + Playwright (Page Object Model)
- **CI:** GitHub Actions (in progress) / Azure Pipelines

### Structure
- `tests/api/` — API autotests against public REST API
- `tests/ui/` — UI autotests (Playwright + POM)
- `pages/` — Page Objects

### How to run locally
```bash
python -m venv venv
source venv/bin/activate          # Windows: venv\Scripts\activate
pip install -r requirements.txt
pytest -v
