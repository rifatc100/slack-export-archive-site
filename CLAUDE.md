# CLAUDE.md — slack-export-archive-site

## Scope
Static marketing site only. No backend, no framework, no build step.

## Hard Rules
- Do NOT introduce JS frameworks, bundlers, or package managers
- Do NOT add tracking, analytics, cookies, or any third-party scripts
- Do NOT mention AI, "AI-powered", or any AI buzzwords
- Do NOT add server-side logic of any kind
- Keep everything deployable as plain static HTML/CSS — no compilation required

## Stack
- `index.html` — single page, all content
- `styles.css` — all styles, no preprocessors
- `assets/` — images, icons, static files only

## Goals
1. **Fast load** — no blocking scripts, minimal CSS, no web fonts from CDNs
2. **Clear copy** — direct, jargon-free language for IT admin and compliance buyers
3. **High trust** — no dark patterns, no fake urgency, no inflated claims

## Buyer Persona
Primary: IT admins and compliance teams running Slack exports
Secondary: Legal/internal counsel handed an archive to review
Not: casual users, developers browsing GitHub, HR generalists

## Tone
- Direct and technical, not salesy
- Honest about what the tool does and does not do
- No superlatives ("best", "powerful", "revolutionary")

## Outputs
Every change must produce a valid, deployable set of:
- `index.html`
- `styles.css`
- `assets/` (if needed)
- `README.md` with Cloudflare Pages deploy steps