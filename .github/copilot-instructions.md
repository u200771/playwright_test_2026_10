# Playwright UI Test Conventions

- Write UI specs in `tests/` using TypeScript and `@playwright/test`.
- Prefer semantic locators such as `getByRole` and web-first `expect` assertions.
- Keep tests independent and use the shared configuration in `playwright.config.ts`.
- Run `npm test` for the full browser suite or `npm run test:ui` for interactive debugging.
- Record a starter flow with `npm run codegen -- <app-url>`, then review and refine the generated test before committing it.
