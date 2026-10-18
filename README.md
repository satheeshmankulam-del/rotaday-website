# RotaWake website

Static site for **RotaWake — Shift Work Calendar** (`com.satheesh.roster`).

Live at https://rotawake.netlify.app

## Structure

```
.
├── index.html                          home
├── 404.html                            not found (Netlify serves automatically)
├── robots.txt
├── sitemap.xml
├── assets/
│   └── og-image.png                    1200x630 social preview
├── faq/index.html
├── support/index.html
├── privacy/index.html                  linked from inside the app
└── 4-on-4-off-shift-calendar-app/      SEO landing page
    └── index.html
```

## Deploying

Push to the `main` branch. Netlify builds from the repository root with no
build command — every file is static.

## Notes

- `privacy/index.html` is the URL registered in Play Console and hard-coded in
  the app at `PRIVACY_URL` in `App.jsx`. Do not move it.
- Each page carries its own inline CSS, so there is no stylesheet to keep in
  sync and nothing to build.
- Add a new rotation landing page by copying
  `4-on-4-off-shift-calendar-app/` and adding the URL to `sitemap.xml`.
