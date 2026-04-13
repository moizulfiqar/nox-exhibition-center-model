# NOX Exhibition Center — Unit Economics Model

A simple **browser-based financial model** for an exhibition venue. Everything runs in one HTML page: you move sliders, and revenue, costs, EBITDA, multi-year views, investment metrics, real-estate comparisons, and cash flow update immediately.

## What it does

- **Dashboard** — KPIs, lease coverage, charts (waterfall, contribution, trends).
- **P&L Model** — Venue pricing, operating assumptions, annual P&L in SAR.
- **Investment** — Capex build-up, payback-style views, discounting helpers.
- **5-Year Forecast** — Occupancy and attach rates by year.
- **Real Estate** — Rent, efficiency, benchmarks against sample venues.
- **Cash Flow** — Monthly and annual cash views for the first years.

Assumptions are **not** sent to a server; all calculations run in your browser. You can **Export** settings as JSON and **Import** them again (see `nox_exhibition_settings-2.json` for an example bundle).

## How to run it locally

1. Clone or download this repository.
2. Open **`index.html`** in a modern browser (Chrome, Safari, Edge, Firefox).

The page loads **Chart.js** from a public CDN, so an internet connection is required for charts.

## Deploy (for example Vercel)

This repo is static: **`index.html`** at the project root, plus **`NOX-Group-logo.png`**. Connect the repository to [Vercel](https://vercel.com), use the default static settings (no build command), and deploy. The app will be served at the root URL.

## Files

| File | Role |
|------|------|
| `index.html` | Main app (same model as `nox_exhibition_center_v9_7.html`, with header branding). |
| `NOX-Group-logo.png` | Logo used in the header and favicon. |
| `nox_exhibition_settings-2.json` | Example exported scenario (import via the app). |
