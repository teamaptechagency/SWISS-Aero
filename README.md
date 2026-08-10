# Swiss Aero Accountancy — Site

Static multi-page site (no build step). Pages are plain HTML that load a small
client-side runtime (`support.js`, `image-slot.js`) directly in the browser.

## Pages

- `index.html` — public marketing site (home)
- `admin.html` — admin panel
- `client-portal.html` — client portal
- `About.dc.html`, `Contact.dc.html`, `Insights.dc.html`, `Pricing.dc.html`,
  `Quote.dc.html`, `Services.dc.html` — public site subpages
- `SiteHeader.dc.html`, `SiteFooter.dc.html` — shared header/footer components,
  loaded at runtime via `<dc-import>`
- `uploads/` — site images

## Run locally

Any static file server works, e.g.:

```bash
npx serve .
```

Then open `http://localhost:3000`.

## Deploy to Vercel

1. Push this folder to a GitHub repo.
2. In Vercel, "Add New… → Project" and import the repo.
3. Framework preset: **Other** (no build command, no output directory needed).
4. Deploy.

Or deploy straight from the CLI:

```bash
npx vercel
```
