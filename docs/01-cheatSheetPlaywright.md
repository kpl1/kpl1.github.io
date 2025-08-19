# Playwright

---


## Commands


```terminal
  $|npx playwright test
  $|npx playwright show-report
  $|npx playwright test --project=chromium --debug
  $|npx playwright test --ui
  $|npx playwright test --headed --project=chromium
  $|npx playwright test -g @Test
  $|npx playwright test --project=chromium --workers=1 --trace on
  $|npx playwright test --workers=1 --trace on
  $|npx playwright test --grep '@P1'
  $|npx playwright test --grep '(?=.*@P1)(?=.*@P2)'
  $|npx playwright test --trace on
```

## Assertion

- version 1.51 - `.filter({visible: true})`
  - getByRole check for visiblity
  - getByText does not check for visibility
    - `await page.getByText(”Hello”).filter({visible: true}).click()`
    - `.filter({ hasText: 'Product 2' }).click()`
- [https://playwright.dev/docs/test-assertions#expecttopass](https://playwright.dev/docs/test-assertions#expecttopass)

- [https://playwright.dev/docs/network#glob-url-patterns](https://playwright.dev/docs/network#glob-url-patterns)
- [https://playwright.dev/docs/api/class-locator#locator-filter](https://playwright.dev/docs/api/class-locator#locator-filter)

**Rooting Url:**

- A single matches any characters except `/`
- A double `*` matches any characters including `/`

[https://playwright.dev/docs/api/class-route](https://playwright.dev/docs/api/class-route)

- Fixture option
  - https://playwright.dev/docs/test-fixtures#fixtures-options
- https://playwright.dev/docs/api/class-apirequestcontext

```tsx
console.log(response.request().url);
console.log(response.request().method());
console.log(response.status());
```
## Locator

- see official documentation [locators](https://playwright.dev/docs/locators)

## Page Object Model

- learn about [playwright-page-object-model](https://www.lambdatest.com/learning-hub/playwright-page-object-model)

## Related link
- [Framework comparison](https://www.checklyhq.com/blog/cypress-vs-selenium-vs-playwright-vs-puppeteer-speed-comparison/)