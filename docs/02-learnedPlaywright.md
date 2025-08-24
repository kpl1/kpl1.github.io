# Playwright

---

## 1.55 : testStepInfo 

- New Property [testStepInfo.titlePath](https://playwright.dev/docs/api/class-teststepinfo#test-step-info-title-path) Returns the full title path starting from the test file, including test and step titles.

## 1.51:  Filter

```js
.filter({visible: true})
.getByRole check for visiblity
.getByText does not check for visibility
await page.getByText(”Hello”).filter({visible: true}).click()
.filter({ hasText: 'Product 2' }).click()
```
- [https://playwright.dev/docs/api/class-locator#locator-filter](https://playwright.dev/docs/api/class-locator#locator-filter)

## URL

**Rooting Url:**

- A single matches any characters except `/`
- A double `*` matches any characters including `/`

- [https://playwright.dev/docs/api/class-route](https://playwright.dev/docs/api/class-route)
- [https://playwright.dev/docs/network#glob-url-patterns](https://playwright.dev/docs/network#glob-url-patterns)

## Fixture

- [Test-fixtures#fixtures-options](https://playwright.dev/docs/test-fixtures#fixtures-options)
- [Class-apirequestcontext](https://playwright.dev/docs/api/class-apirequestcontext)

## Locator

- see official documentation [locators](https://playwright.dev/docs/locators)

## Assertion

- [Test-assertions#expecttopass](https://playwright.dev/docs/test-assertions#expecttopass)

```js
await expect(async () => {
  const response = await page.request.get('https://api.example.com');
  expect(response.status()).toBe(200);
}).toPass();
```

## Page Object Model

- learn about [playwright-page-object-model](https://www.lambdatest.com/learning-hub/playwright-page-object-model)

## Related link
- [Framework comparison](https://www.checklyhq.com/blog/cypress-vs-selenium-vs-playwright-vs-puppeteer-speed-comparison/)