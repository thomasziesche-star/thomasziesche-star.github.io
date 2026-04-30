# thomasziesche-star.github.io

Static landing page for **Accountant with beard**, an independent
mobile-app-development practice operated by Thomas Ziesche from Germany.

The page exists primarily as the **developer website** required by Google
Play for organisation-account verification (DUNS-bound).

## Structure

- `index.html` — landing page (English)
- `impressum.html` — legal notice per § 5 TMG (German, required by law)
- `datenschutz.html` — privacy policy per GDPR (German, required by law)
- `styles.css` — shared minimal styling, light/dark via
  `prefers-color-scheme`

No build step. Plain static HTML; deployed via GitHub Pages from `main`.

## Local preview

Any static file server works. Easiest:

```bash
python -m http.server 8000
```

Then open http://localhost:8000/.

## Deployment

GitHub Pages serves the repository root of `main`. Configured under
**Settings → Pages**.

Live at: https://thomasziesche-star.github.io/

## Maintenance

- Update copyright year: handled automatically via JavaScript in the
  footer of each page.
- Update apps section: edit the `#apps` block in `index.html`.
- Legal pages should be reviewed yearly, or whenever the underlying
  business situation changes (address, legal form, contact email).
