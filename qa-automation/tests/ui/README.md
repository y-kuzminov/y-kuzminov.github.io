# UI Autotests

pytest + Playwright with Page Object Model against saucedemo.com.

**Covered:** successful login, locked-out user error, add product to cart.

Run:
    pip install -r ../../requirements.txt
    playwright install
    pytest tests/ui -v
