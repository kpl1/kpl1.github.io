# Playwright

---


###  Commands


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

### Console log

```tsx
console.log(response.request().url);
console.log(response.request().method());
console.log(response.status());
```
