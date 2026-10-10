# Playwright UI Tests

TypeScript end-to-end UI tests powered by Playwright Test. The starter tests exercise the Playwright documentation site; replace those flows with your application's URL and workflows.

## Run tests

```bash
npm test
npm run test:ui
npm run test:headed
```

## Record a test

Start your application, then run:

```bash
npm run codegen -- http://localhost:3000
```

Use the opened browser to perform the workflow. Playwright writes the recorded test to `tests/recorded.spec.ts`; review the generated locators and add assertions before relying on it.

## Browsers

The project is configured for Chromium, Firefox, and WebKit. Install the matching browser binaries with:

```bash
npx playwright install
```
