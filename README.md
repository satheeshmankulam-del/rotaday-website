# RotaWake website

Static site for **RotaWake — Shift Work Calendar** (`com.satheesh.roster`).
Live at https://rotawake.netlify.app. Structured to match linkedbookmark.netlify.app.

## Structure

```
.
├── index.html                          home
├── 404.html
├── robots.txt
├── sitemap.xml
├── assets/
│   ├── favicon.svg  favicon-32.png  apple-touch-icon.png  icon-512.png
│   ├── og-image.png                    1200x630 social preview
│   └── screen-*.png                    six app screenshots, 780x1560
├── faq/index.html                      15 questions in 4 groups, FAQPage schema
├── support/index.html
├── privacy/index.html                  linked from inside the app
└── 4-on-4-off-shift-calendar-app/      SEO landing page
    └── index.html
```

## Deploying

Push to `main`. Netlify builds from the repository root with no build
command — every file is static.

## Notes

- `privacy/index.html` is the URL registered in Play Console and hard-coded
  in the app at `PRIVACY_URL` in `App.jsx`. Do not move it.
- Colours come from the theme object `T` and `PALETTE` in `App.jsx`. If the
  app's palette changes, update `:root` to match.
- Screenshots in `assets/` are rendered from the same mockups as the Play
  Store images, so the two never drift apart.
- Add a rotation landing page by copying `4-on-4-off-shift-calendar-app/`
  and adding its URL to `sitemap.xml`.
