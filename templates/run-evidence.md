# Run evidence — Add car

- Tool: Terminal (output provided by user)
- Command: `npx playwright test tests/add-car.spec.ts --project=chromium`
- Timestamp: Not provided
- Environment: Playwright Chromium; host and OS not stated
- Actual output (verbatim):

```text
npm notice run npx
npm notice run 'playwright' test tests/add-car.spec.ts --project=chromium

Running 1 test using 1 worker

  ✓  1 [chromium] › tests/add-car.spec.ts:3:5 › guest can add an Audi TT to Garage (2.2s)

  1 passed (2.7s)

To open last HTML report run:

  npx playwright show-report
```

| Елемент | Джерело |
|---|---|
| setup | `playwright.config.ts`: `baseURL` and Chromium project |
| locator/action | Current UI verified in the approved Playwright CLI inspection: `Guest log in`, `Add car`, `Brand`, `Model`, `Mileage`, `Add` |
| assertions | `specs/add-car.md`: Garage URL and visible `Audi TT` after saving |

- FACTS: The provided terminal output shows `1 passed (2.7s)`.
- ASSUMPTIONS: None.
- RISKS: Timestamp and host OS were not included in the provided output.
- HUMAN CORRECTION: None.
- DECISION: `ACCEPT` — the provided Playwright output records one passing test.
