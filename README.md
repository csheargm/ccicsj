# CCIC San Jose — Demo Site

A bilingual (English / Traditional Chinese / Simplified Chinese) demo homepage for
CCIC San Jose (Chinese Church In Christ), built from the church's existing public
content (history, beliefs, mission/vision/values, service times, ministries, giving,
and missions calendar from ccic-sj.org).

**This is a draft/demo site for elder board review — not the live church website.**

## What's here

- Single static `index.html` — no build step, deploy anywhere (GitHub Pages, S3, etc.)
- Language toggle (EN / 繁 / 简) driven by one flat `CONTENT` object in the page's
  own script — the shape a headless CMS or an AI content-update agent would read
  and write field-by-field
- Two demo-only, client-side-simulated capabilities (no real backend):
  - **"Ask CCIC"** — a visitor-facing FAQ chat widget answering from the same
    content model that renders the page
  - **"Staff: AI Content Agent"** — a staff-facing demo showing an AI agent
    drafting a content change, staging it for elder approval, and publishing it
    live on approval

## Local preview

Just open `index.html` in a browser, or serve it:

```bash
python3 -m http.server 8080
```

## Deploy

Published via GitHub Pages from the `main` branch root.
