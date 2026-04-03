# adamwollins.com.au — Editing Guide

## File structure
```
style.css          ← Shared styles — edit colours/fonts here
index.html         ← Homepage / welcome
cv.html            ← Full CV
ict-strategy.html  ← ICT Strategy for Schools
sitemap.xml        ← Update when adding new pages
robots.txt         ← Leave as-is
```

## Adding a new page
1. Copy any existing page (e.g. `cv.html`) as your template
2. Update the `<title>` and `<meta name="description">` tags
3. Add a `<li><a href="your-page.html">Page Name</a></li>` to the `nav-links` list in ALL pages
4. Add the URL to `sitemap.xml`
5. Link to it from the homepage section cards if appropriate

## Updating content
- **Homepage hero text**: Edit the `<h1>` and `.hero-sub` paragraph in `index.html`
- **CV bullet points**: Find the relevant `<ul class="bullet-list">` in `cv.html`
- **Services**: Each `<div class="service-card">` in `ict-strategy.html` is one service
- **Articles**: Replace the `<div class="placeholder-card">` blocks as articles are written

## Key design tokens (in style.css)
- `--accent: #c96442` — terracotta, the main brand colour
- `--bg: #f5f4ef` — warm cream background
- `--font-display: 'Fraunces'` — headings
- `--font-body: 'Plus Jakarta Sans'` — all body text

## Deploying
Upload all files in this folder to the root of your web host.
No build step required. Everything runs as static HTML.
