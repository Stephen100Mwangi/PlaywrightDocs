# Playwright

Playwright is a framework for Web Testing and Automation. It allows you to write tests that run across all modern web browsers.

## Installation

Install Playwright using npm:

```
npm install @playwright/test
```

## Usage

Create a test file, e.g., `tests/example.spec.js`:

```javascript
const { test, expect } = require('@playwright/test');

test('basic test', async ({ page }) => {
  await page.goto('https://playwright.dev/');
  const title = page.locator('h1');
  await expect(title).toContainText('Playwright');
});
```

Run the tests:

```
npx playwright test
```

## Documentation

For more details, visit the [official Playwright documentation](https://playwright.dev/docs/intro).