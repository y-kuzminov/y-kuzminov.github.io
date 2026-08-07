# UI Autotests

pytest + Playwright with Page Object Model against saucedemo.com.

**Covered:**
- Successful login
- Locked-out user error
- Add product to cart

**Run:**
```bash
pip install -r ../../requirements.txt
playwright install
pytest tests/ui -v
