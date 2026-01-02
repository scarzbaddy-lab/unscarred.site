# Unscarred.site

Unscarred.site is a static website for Unscarred tools, scans, and interactive pages.
Built to deploy automatically via Netlify when changes are pushed to GitHub.

## What’s inside
- Static pages (landing pages, program pages, resources)
- Interactive scans and quizzes (HTML, CSS, JS)
- Reusable site styling (shared CSS)
- Optional local history storage for quiz results (browser localStorage)

## Tech
- HTML, CSS, Vanilla JS
- Netlify deploys from this GitHub repo

## Project structure (update if yours differs)
Common layouts:
- `index.html` or `/index.html` is the homepage
- `/pages/` contains routed pages
- `/assets/` contains styles, scripts, and images

Example:
- `assets/styles.css`
- `assets/app.js`
- `pages/nervous-system-scan/index.html`

## Local development
Option A: VS Code Live Server
1. Open the repo in VS Code
2. Install “Live Server”
3. Right click `index.html` and select “Open with Live Server”

Option B: Simple local server (Node)
1. `npm i -g serve`
2. `serve .`
3. Open the local URL it prints

## Deployment
Netlify is connected to this repo.
Every push to the default branch triggers a deploy.

If you use a `netlify.toml`, Netlify will follow its build and publish settings.

## How to add a new page
Recommended pattern for clean URLs:
- Create a folder inside `/pages/`
- Put an `index.html` inside it

Example:
- Route: `/nervous-system-scan/`
- File: `pages/nervous-system-scan/index.html`

Checklist:
1. Copy header and footer from an existing page so styling stays consistent
2. Add the new route to navigation (header and footer links)
3. Keep links relative and working on Netlify
4. Test locally, then push

## How to add a new quiz or scan
1. Duplicate an existing quiz page as a starter
2. Update:
   - Page title and meta description
   - Questions array and scoring logic
   - Result copy and CTAs
3. Keep shared styles and buttons consistent

## Content and brand
- Brand: Unscarred
- Tone: clear, grounded, emotionally honest
- Design: dark luxe, soft accent highlights
Update any palette or font decisions in the main stylesheet so everything stays unified.

## Copilot guidance (optional but recommended)
If you want GitHub Copilot to build pages consistently, add:
- `.github/copilot-instructions.md`

Keep it focused on:
- Where pages live
- How to reuse header and footer
- How to add routes
- No new frameworks unless requested

## Contributing
- Keep changes small and readable
- Do not introduce new dependencies unless necessary
- Favor accessibility: semantic HTML, keyboard usable buttons, good contrast, readable fonts

## License
All rights reserved unless you add a license file.

## Contact
Owner: Unscarred
Site: https://unscarred.site
