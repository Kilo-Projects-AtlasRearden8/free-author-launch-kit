# STATUS

## What was built

A free, no-account-required author launch kit for Dylan Asdale / Asdale Dynamics, LLC. Each tool exists as both a fillable printable HTML page and a printable Markdown document. Everything runs locally in the browser; nothing is uploaded, stored, or requires a sign-up.

Tools included (5):

| Tool | HTML | Markdown | Purpose |
|------|------|----------|---------|
| Book Launch Checklist | `launch-checklist.html` | `launch-checklist.md` | Step-by-step pre-launch, launch-week, and post-launch tasks with checkboxes |
| Press Release Template | `press-release.html` | `press-release.md` | Fill-in-the-blanks press release for blogs, newsletters, and media |
| ARC Reader Tracker | `arc-reader-tracker.html` | `arc-reader-tracker.md` | Track advance reader copies sent and reviews coming back |
| Review Log | `review-log.html` | `review-log.md` | Log reviews, ratings, quotes, and thank-you follow-ups |
| Social-Post Planner | `social-post-planner.html` | `social-post-planner.md` | Plan and schedule posts across platforms with hashtags and links |

Supporting files:

- `LICENSE` — MIT License, copyright line exactly `Copyright (c) 2026 Asdale Dynamics, LLC`
- `README.md` — kit overview, how to use, audience, credit to Asdale Dynamics, LLC, license
- `STATUS.md` — this file

## Credit

Built and published by Asdale Dynamics, LLC (Indiana, formed October 2026). Every HTML and Markdown tool credits Asdale Dynamics, LLC, and the README credits Asdale Dynamics, LLC.

## How to run

No install, no account, no internet needed after download.

1. Open any `.html` file in a browser (Chrome, Firefox, Safari, Edge).
2. Fill in the fields on screen.
3. Press `Ctrl+P` (Windows/Linux) or `Cmd+P` (Mac) to print. A dedicated print stylesheet strips buttons and shows clean, fillable worksheets. Save as PDF for a digital copy.
4. The `.md` files can be printed directly or edited in any text editor.

All files are standalone — open any one independently. No build step, no dependencies, no external CDN.

## Verification results

A Python verification script checked all 13 expected files. Results:

- All 13 expected files present: PASS
- No `.github/workflows` directory: PASS
- `LICENSE` starts with `MIT License` and contains the exact line `Copyright (c) 2026 Asdale Dynamics, LLC`: PASS
- `README.md` credits Asdale Dynamics, LLC: PASS
- All 5 HTML files parse without tag mismatches: PASS
- All 5 HTML files credit Asdale Dynamics, LLC and include a copyright line: PASS
- All 5 HTML files contain fillable `<input>`/`<textarea>` fields: PASS
- All 5 HTML files include an `@media print` stylesheet: PASS
- All 5 Markdown files credit Asdale Dynamics, LLC and include a copyright line: PASS
- Credential/token scan (API keys, credentials, access tokens): PASS — the only flagged fragment was a hyphenated piece inside the harmless CSS class name `task-text`; neither is an actual key or personal data.

## Known gaps

- The HTML tools include small inline JavaScript "add row" and "print" buttons for on-screen convenience; these buttons are hidden when printed. Nothing requires JavaScript to use the worksheets.
- Each HTML file embeds its own CSS (no shared stylesheet), so styles are duplicated across the 5 files. This keeps every file standalone and shareable.
- No automated test suite or lint config is included; verification is via the one-off Python check above.
- The kit is a static freebie — no backend, no accounts, no data collection, and no tracking.
- Not yet committed to git at time of writing (to be committed after this status note).
