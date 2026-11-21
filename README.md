# ACCT 65023 Live Workbook

An Excel-style study workbook for TCU Neeley EMBA ACCT 65023 (Managerial Accounting), Sessions 1, 2 and 6. It runs entirely in the browser: one `index.html`, no build step, no server code.

## What it does

- Live sheets for each Session 1, 2 and 6 case (Session 6: Hospitality Inns ROI/RI, Tri-Cities Community Bank, Marlow Diagnostics July and August variances): blue cells are inputs, and every formula recalculates when you change one.
- Click any result to see its formula as cell references, in words, and with the numbers plugged in.
- Practice mode hides worked answers and checks the answers you type.
- Goal Seek, Show formulas (Ctrl + `), and Copy with formulas (pastes into Excel at A1).
- CVP template, incremental-decision template, and a blank scratch sheet for new problems.

Edits and practice answers are saved in your browser's local storage only.

## Session 6 Tools

- [Variance Dashboard](variance-dashboard/): Marlow Diagnostics July and August budget vs. actual: flexible budget, market-size and market-share variances, price and quantity variances, flags, waterfall and upload buttons for new files.
- [Balanced Scorecard](balanced-scorecard/): Amethyst Pediatric Therapy strategy map, measures, editable targets and status, weakest-link test, 90-day plan and improved AI prompts.

## Publish with GitHub Pages

1. Create a new repository on GitHub (for example `acct-65023-live-workbook`).
2. Upload `index.html`, `README.md`, and `.nojekyll` to the root of the repository (Add file → Upload files, then Commit).
3. Go to **Settings → Pages**. Under **Build and deployment**, set **Source** to *Deploy from a branch*, choose branch `main` and folder `/ (root)`, then **Save**.
4. After a minute or two the site is live at `https://<your-username>.github.io/<repository-name>/`.

Or from a terminal:

```bash
git init
git add index.html README.md .nojekyll
git commit -m "Add ACCT 65023 live workbook"
git branch -M main
git remote add origin https://github.com/<your-username>/<repository-name>.git
git push -u origin main
```

Then turn on Pages as in step 3.

## Updating

Replace `index.html` with the new version and commit. Pages redeploys automatically.

## External resources

Each page loads only the Inter font from Google Fonts. Everything else is inline (the variance dashboard inlines SheetJS 0.18.5, Apache-2.0, to read uploaded .xlsx files).
