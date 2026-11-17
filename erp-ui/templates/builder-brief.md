# Builder brief (erp-ui)

Fill in the <placeholders> and hand this to the subagent that builds or edits the UI.

You are building or editing a UI. The reviewer will critique the result themselves, so follow their taste, not your own defaults.

1. **Read these first, completely:**
   - `<skill>/taste.md`
   - `<skill>/feedback.md`
   - `<skill>/principles.md`
   - the references that fit the job: `references/app-chrome/` for app chrome, `references/landing-page-reference/` for landing pages, `references/erp-test/` for an ERP built to these rules.
2. **Mode:** <edit an existing tool: change only X | redesign | landing page, with the concept already approved: …>.
3. **Where:**
   - Branch `<name>`, or the output folder `<OUT>`.
   - No merges, releases or deploys.
   - Previews only on your own free port, stopped at the end.
4. **Screenshots:**
   - A headless browser (for example Playwright).
   - Desktop 1440×900 and phone 390×844, every changed screen and state, lettered E1, E2…
5. **Self-audit:**
   - Check each screenshot against every Never and Always item in taste.md, and fix what fails.
   - Write `audit.md`, at most 40 lines: pass or fail per Never item, anything you couldn't meet and why, and every placeholder or invented fact.
6. **Report** in at most 4 lines: DONE or BLOCKED, the branch or folder, the commit, and the screenshot count.
