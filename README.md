# Vanderbilt Ave Street Infrastructure Stroll

A static website version of Chris Whong's "Vanderbilt Ave Street Infrastructure Stroll" (17 July 2022) — a 26-stop field guide to everyday urban infrastructure along Vanderbilt Avenue in Prospect Heights, Brooklyn.

## What this is

Plain HTML, CSS, and a few lines of vanilla JS (smooth-scroll table of contents, click-to-zoom lightbox). No build step, no framework, no dependencies — open `index.html` directly or drop the folder on any static host. This keeps it working indefinitely with zero maintenance.

## Structure

```
index.html   — the whole site
images/      — all photos and diagrams, extracted from the original PDF
robots.txt   — allows search engine indexing
```

## Hosting it

This repo deploys automatically to GitHub Pages via the workflow in `.github/workflows/deploy.yml` on every push to `main`. The first time this is set up, go to the repo's **Settings → Pages** and set the source to **GitHub Actions** (only needs doing once).

It's also just static files, so any of these work with no configuration:

- **Netlify / Cloudflare Pages**: drag-and-drop the folder in their web dashboard.
- **Anywhere else**: copy the files to any web server.

To preview locally: `python3 -m http.server 8000` from this directory, then visit `http://localhost:8000`.

## Content notes

- Photos and diagrams are reproduced from the original PDF; each one links back to its original source where the PDF cited one.
- Stops 21–25 had no photo in the original document, so the site shows title-only entries for them, matching the source.
- The map graphic and its numbered labels are rendered as a single image, matching the original page 1 layout.
