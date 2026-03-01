# SlackExportArchive — Landing Page

Static marketing site for [SlackExportArchive](https://github.com/rifatc100/slack-export-archive): turn a Slack export ZIP into a searchable, offline HTML archive.

## Structure

```
slack-export-archive-site/
├── index.html      # Main landing page
├── styles.css      # Styles
├── assets/
│   ├── quick_demo.mp4  # Demo video
│   └── screenshot.png  # Screenshot
└── README.md
```

## Local preview

```bash
npx serve .
```

Or open `index.html` directly in a browser.

## Deploy to Cloudflare Pages

### Option 1: Connect a Git repository

1. Go to [Cloudflare Dashboard](https://dash.cloudflare.com) → Pages → Create a project.
2. Connect your Git provider (GitHub, GitLab) and select this repo.
3. Configure build settings:
   - **Build command:** Leave empty (no build step).
   - **Build output directory:** `/` (root).
4. Deploy. Cloudflare will serve the static files from the repo root.

### Option 2: Direct upload (Wrangler)

```bash
npx wrangler pages deploy . --project-name=slack-export-archive
```

### Custom domain

In the Cloudflare Pages project → Custom domains → Add a domain and follow the DNS instructions.

## Requirements

- Static HTML/CSS only. No build step, no framework.
- Ensure `assets/quick_demo.mp4` and `assets/screenshot.png` exist for full functionality.
