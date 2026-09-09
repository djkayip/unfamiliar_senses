# unfamiliar_senses — static site

Pre-built static export of an Obsidian vault (graph + notes browser).
All paths are relative, so this works at any URL without reconfiguration.

## Deploy to GitHub Pages

1. Push this folder's contents to the **main** branch of `djkayip/unfamiliar_senses`.
2. In the repo: **Settings → Pages → Build and deployment → Source: GitHub Actions**.
3. The included workflow (`.github/workflows/deploy.yml`) publishes on every push.

Site URL: https://djkayip.github.io/unfamiliar_senses/

## Local preview

This is a single-page app that `fetch`es JSON data, so it needs an HTTP
server (opening index.html via file:// is blocked by browser CORS):

    npx serve .        # or: python3 -m http.server 8000
