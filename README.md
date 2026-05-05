# Academic Portfolio Website

A clean static one-page portfolio for a research fellow working at the intersection of peace and conflict data, engineering, visualization, and NLP.

## Quick Start

Open `index.html` in a browser.

## Run on Localhost (Recommended)

From the project folder, run:

```powershell
python -m http.server 5500
```

Then open:

`http://localhost:5500`

## Theme Toggle

- A header toggle switches between light and dark mode.
- The selected mode is stored in `localStorage`, so visitors keep their preference.
- If no saved preference exists, the site follows system theme.

## Easy Updates

- Main content cards are in `script.js` inside the `siteContent` object.
- Contact links are in `index.html` under the `#contact` section.
- Colors and typography are controlled in `styles.css` under `:root`.

## Suggested Next Edits

1. Replace `Your Name` and email in `index.html`.
2. Replace `#` links in `script.js` with your real project, dataset, and publication URLs.
3. Optional: add a CV link in the header or contact section.
