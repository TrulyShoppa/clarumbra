# Clarumbra

AI visibility & compliance platform — marketing site and live discovery-scan demo. Static, no build step, no backend, no dependencies beyond Google Fonts loaded over the network.

## What's here

- `index.html` — the marketing/landing page (corona-reveal hero, pricing, features).
- `dashboard.html` — the live Track 1 demo: upload a Google Workspace / Microsoft 365 app-access export (or load sample data), and it's scanned and risk-scored entirely in the browser. No server, no upload, no backend.

## Preview locally

Just open `index.html` in a browser. No install, no server needed.

## Deploy — pick one

**GitHub Pages (free)**
1. Push this repo to GitHub.
2. Repo → Settings → Pages → Source: deploy from branch → `main` / root.
3. Site goes live at `https://<username>.github.io/<repo>/`.
4. Custom domain: same Pages settings screen → add your domain, then create the CNAME/A record your DNS provider tells you to at your domain registrar.

**Netlify or Vercel (free)**
1. Drag-and-drop this folder onto netlify.com/drop, or connect the GitHub repo for auto-deploy on every push.
2. Custom domain: Site settings → Domain management → add your domain, then point DNS as instructed.

## Notes

- Both pages share one design system (colors/fonts defined as CSS variables at the top of each `<style>` block) — edit in both files if changing the palette or type.
- `dashboard.html` has a small built-in risk database (~45 known AI tools) as a JS array near the bottom of the file — that's the easiest place to add more tools or adjust risk levels as you learn more.
- Trial/CTA buttons are wired to route between the two pages but don't yet post anywhere — connect a real signup capture (e.g., a form service, or your own backend) when ready.
