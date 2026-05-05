# Niamh Henry Website

Static portfolio site for `niamhhenry.com`.

This site is deployed from GitHub Pages using the repository:
`https://github.com/niamhhenry/nhen_website`

## Project Structure

- `index.html`: Page structure, section layout, navigation, contact block
- `styles.css`: Design system, responsive layout, theme styles
- `script.js`: Portfolio content model (`siteContent`) and card rendering
- `assets/`: Images (project screenshots + headshot)
- `CV_CONTENT.md`: CV source content in markdown
- `CNAME`: Custom domain for GitHub Pages (`niamhhenry.com`)

## Edit Content

Most text content is in `script.js`.

1. Open `script.js`
2. Edit entries inside the `siteContent` object (`featured`, `collaborations`, `datasets`, `publications`, `recognition`, `education`, `wip`)
3. Save and preview locally

Use these fields in each item:

- `meta`: short tag above card title
- `title`: card title
- `description`: 1-2 sentence summary
- `linkLabel`: button/link text
- `linkUrl`: destination URL
- `image` (optional): image path like `assets/tracker.png`
- `secondaryLink` (optional): `{ label: "...", url: "..." }`

## Edit Layout or Styling

- Update page structure and section order in `index.html`
- Update colors, spacing, typography, and responsive behavior in `styles.css`

## Run Locally

From `c:\Users\nhenry2\website`:

```powershell
python -m http.server 5500
```

Open `http://localhost:5500`

## Redeploy After Changes

GitHub Pages redeploys automatically whenever you push to `main`.

From `c:\Users\nhenry2\website`:

```powershell
git add .
git commit -m "Update website content"
git push
```

That is all you need for normal updates.

## One-Time GitHub Pages Setup (Already Completed Once)

If you ever need to reconfigure:

1. GitHub repo -> Settings -> Pages
2. Source: `Deploy from a branch`
3. Branch: `main` and folder: `/(root)`
4. Custom domain: `niamhhenry.com`
5. Enable `Enforce HTTPS` once certificate is issued

## DNS Records for Domain

At your registrar, ensure these records exist:

- `A` host `@` -> `185.199.108.153`
- `A` host `@` -> `185.199.109.153`
- `A` host `@` -> `185.199.110.153`
- `A` host `@` -> `185.199.111.153`
- `CNAME` host `www` -> `niamhhenry.github.io`

## Notes

- `CNAME` file must remain in the repo root for custom domain mapping.
- First publish or DNS changes can take a little time to propagate.
- If a page looks stale, hard refresh your browser.
