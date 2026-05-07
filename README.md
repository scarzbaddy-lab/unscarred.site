# unscarred.site

Static site for Unscarred, deployed on Netlify.

## How this repo is structured

This repo is a plain HTML site. Every route is a folder with an `index.html`.

Examples:

- `/about/` → `about/index.html`
- `/quiz/` → `quiz/index.html` (main quiz hub)
- `/quiz/nervous-system-response/` → `quiz/nervous-system-response/index.html`
- `/quiz/are-they-hurting-me/` → `quiz/are-they-hurting-me/index.html`
- `/war/` → `war/index.html` (war room hub)

Individual quizzes can also be flat HTML files: `/quiz/something.html` → `quiz/something.html`

Netlify serves `index.html` automatically for each folder route.

## Local preview

Use any static server. Two easy options:

### Option 1: VS Code Live Server
Open the repo in VS Code and run Live Server.

### Option 2: Python
```bash
python -m http.server 8888
```
Then open `http://localhost:8888`.

## Add a new page

1. Create a folder for the route.
2. Add `index.html` inside it.
3. Use root absolute links so they work anywhere:

- Good: `/about/`
- Avoid: `../about/` or `about.html`

## Navigation rules

- The header must always include these links in this order:
  1. Quizzes → `/quiz/`
  2. War Room → `/war/`
  3. About → `/about/`
- Use root absolute links only: `/about/` not `about/index.html` and not `../about/`
- Never use `quizzes.html` in new code. Use `/quiz/`

## Netlify

This repo is a static site. No build command required.

Suggested settings:

- Build command: *(empty)*
- Publish directory: `/`

## Notes

Unscarred content is education and pattern support, not diagnosis and not medical, psychiatric, or legal advice.
