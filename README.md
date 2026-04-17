# AI Enablement Status

Weekly status reports from Fourth's AI Enablement Team. Published as a static site via GitHub Pages.

**Live:** https://rev4nchist.github.io/ai-enablement-status/

## Structure

```
/
├── index.html                          # Landing page — lists all reports
├── reports/
│   ├── 2026-02-february/index.html     # Feb 2026 baseline
│   └── 2026-w16-april/index.html       # Week 16 · April 2026
└── .nojekyll                           # skip Jekyll processing
```

## Adding a new weekly report

1. Generate the HTML report (e.g. via the Donna Notion TaskMaster workflow).
2. Create a new folder under `reports/` using the naming convention `YYYY-wNN-month/` (e.g. `2026-w17-april/`).
3. Save the HTML as `index.html` inside that folder.
4. Update the root `index.html` to:
   - Add a new `.report-card` block at the top of the `.reports` list.
   - Move the `.latest` class from the previous top card to the new one.
   - Update the `Latest` meta field in the hero to match the new week.
5. Commit and push to `master` — GitHub Pages rebuilds automatically.

## Naming convention

| Part | Format | Example |
| --- | --- | --- |
| Year | 4 digits | `2026` |
| Week | `w` + ISO week number | `w16` |
| Month | lowercase, for humans | `april` |

Full folder: `reports/2026-w16-april/`

## URLs

| Report | URL |
| --- | --- |
| Landing (always latest) | https://rev4nchist.github.io/ai-enablement-status/ |
| Feb 2026 | https://rev4nchist.github.io/ai-enablement-status/reports/2026-02-february/ |
| W16 April 2026 | https://rev4nchist.github.io/ai-enablement-status/reports/2026-w16-april/ |
