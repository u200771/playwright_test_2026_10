# Run this project on Windows

## What you need

- A supported Windows 10 or Windows 11 computer.
- [Node.js](https://nodejs.org/) (use the current LTS release; npm is included).
- [Git for Windows](https://git-scm.com/download/win).
- [Visual Studio Code](https://code.visualstudio.com/) (optional, but useful for editing and running tests).
- An internet connection to clone the project, install packages and browsers, and visit the websites under test.

## Set up the project

Open PowerShell or the VS Code terminal and run:

```powershell
git clone https://github.com/u200771/playwright_test_2026_10.git
cd playwright_test_2026_10
npm install
npx playwright install
```

`npx playwright install` downloads the Chromium, Firefox, and WebKit browser builds used by this project's Playwright configuration. You only need to run it again when Playwright is updated or a browser build is missing.

## Run tests

Run the tests in all configured browsers:

```powershell
npm test
```

Run just the Chromium tests with a visible browser window:

```powershell
npx playwright test --project=chromium --headed
```

Run just the Chromium tests without showing a browser window:

```powershell
npx playwright test --project=chromium
```

The tests visit public websites, so those sites must be reachable from the computer. The browser started by Playwright is its managed Chromium build; it is not necessarily the separately installed Google Chrome application.

## View the HTML report

After a test run, open the report with:

```powershell
npx playwright show-report
```

## Run tests from VS Code

Open the cloned project folder in VS Code. Install the **Playwright Test for VS Code** extension if you want to run tests from the Testing view. To see a browser window when starting tests from that view, enable **Show Browser** in the Playwright sidebar. You can also run the headed command above in the integrated terminal.
