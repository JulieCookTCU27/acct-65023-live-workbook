# ACCT 65023 Live Workbook

An Excel-style study workbook for TCU Neeley EMBA ACCT 65023 (Managerial Accounting), Sessions 1–2. It runs entirely in the browser: one `index.html`, no build step, no server code.

## What it does

- Live sheets for each Session 1–2 case: blue cells are inputs, and every formula recalculates when you change one.
- Click any result to see its formula as cell references, in words, and with the numbers plugged in.
- Practice mode hides worked answers and checks the answers you type.
- Goal Seek, Show formulas (Ctrl + `), and Copy with formulas (pastes into Excel at A1).
- CVP template, incremental-decision template, and a blank scratch sheet for new problems.

Edits and practice answers are saved in your browser's local storage only.

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

The page loads only the Inter font from Google Fonts. Everything else is inline.
