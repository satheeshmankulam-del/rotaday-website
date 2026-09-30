# Rotaday website

Static site for the Rotaday Android app. No build step: Netlify serves these files as they are.

| Path | Page |
|---|---|
| `index.html` | Home |
| `privacy/index.html` | Privacy policy (use `/privacy/` in Play Console) |
| `faq/index.html` | FAQ |
| `support/index.html` | Support and data deletion |
| `404.html` | "Page not found" page |
| `assets/site.css` | All styles (colours are at the top) |
| `assets/analytics.js` | Microsoft Clarity (paste your ID here) |

## Before publishing
1. `assets/analytics.js`: paste your Clarity Project ID, or leave it empty.
2. If your Netlify site name differs, find and replace `https://rotaday.netlify.app` in every file.
