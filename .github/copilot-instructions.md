# Copilot Instructions for unscarred.site

## Routing
- Quiz hub is `/quiz/` and must be `quiz/index.html`
- Individual quizzes live in `/quiz/` as flat html files like `quiz/name.html` or subdirectories like `quiz/name/index.html`
- War hub is `/war/` and must be `war/index.html`
- Use root absolute links only, starting with `/`

## Header and footer
- Every page must include the same header and footer markup
- Header nav order must be:
  1. `/quiz/` - Quizzes
  2. `/war/` - War Room
  3. `/about/` - About
  4. `/work/` - Work With Me
  5. `/blog/` - Blog

## Link hygiene
- Never link to `quizzes.html` in new changes
- Always link quiz hub as `/quiz/`
- Any back link from a quiz must go to `/quiz/`
- Use root absolute paths: `/quiz/` not `../quiz/` or `quiz/index.html`

## CSS
- Shared CSS lives in `/assets/site.css`
- Pages must load it with `<link rel="stylesheet" href="/assets/site.css">`
- Do not copy large CSS blocks into each page

## Quiz Hub Structure

### /quiz/ hub sections
- Relationship patterns
- Attachment and repair
- Nervous system tools
- Self and identity

### /war/ hub sections
- Harm and control scans
- Reality checks
- Trauma bond stabilization
- Evidence tracking and decision tools
