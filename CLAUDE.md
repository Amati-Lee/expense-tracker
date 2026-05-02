# Expense Tracker

## IMPORTANT: This is a PUBLIC GitHub repo
Repository: `Amati-Lee/expense-tracker`
Deployed to: GitHub Pages (https://amati-lee.github.io/expense-tracker/)

## Tech Stack
- Pure frontend PWA (single `index.html` with inline JS/CSS)
- Data stored in browser `localStorage`
- Encrypted export/import with AES-256-GCM + PBKDF2
- Optional app password lock (stored locally)
- Service Worker for offline support
- No backend, no external API calls

## Security Rules

### Sensitive Information
- NEVER hardcode passwords, keys, tokens, or secrets in source code
- Financial data is stored ONLY in browser localStorage
- `.wrangler/` directory contains Cloudflare account info and MUST be in `.gitignore`
- No `.env` file is needed for this project (pure frontend)

### Before Every Push
1. Run `git status` to verify no unexpected files (especially `.wrangler/`)
2. Confirm no `.env` or backup files are staged
3. Confirm no real financial data or test credentials in code
4. Review `git diff --staged` for any accidental secrets
