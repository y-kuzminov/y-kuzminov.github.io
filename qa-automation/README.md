# Automation

Test automation with Python.

## Stack
Python · pytest · requests (API) · Selenium + Page Object Model (UI) · Azure Pipelines (CI)

## Structure
- `tests/api/` — API autotests (requests + pytest) against reqres.in
- `tests/ui/`  — UI autotests (Selenium + POM) against saucedemo.com
- `pages/`     — Page Objects
- `azure-pipelines.yml` — CI pipeline (runs tests on push)

## How to run locally
    python -m venv venv
    # Windows: venv\Scripts\activate
    pip install -r requirements.txt
    pytest -v

## CI
Tests run automatically in Azure DevOps on each push.
<!-- после первого зелёного билда вставь сюда скриншот: -->
<!-- ![pipeline](./screenshots/azure-green.png) -->
