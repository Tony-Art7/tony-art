# tony-art.com — Starter (Updated)

A lightweight, secure personal site for Tony. Static HTML, deployed on Vercel.

## Quick Start
1. Add these files to the repo.
2. Vercel auto-deploys on push.
3. Domains (GoDaddy DNS):
   - **A @ → 216.198.79.1** (Vercel new IP)
   - **CNAME www → <your project-specific> .vercel-dns-xxx.com** (shown in Vercel)
   - `www` should **308 redirect** to the apex `tony-art.com` in Vercel → Domains.

## Customize
- Replace GitHub URL in `index.html` and add `resume.pdf` at repo root.
- Place your icons in `/assets` and keep `site.webmanifest` at repo root.
- Headshot for social previews: `/assets/headshot.jpg` (ideally 1200×630).

## Security
- Strong headers via `vercel.json`. If you add external scripts/services, update CSP accordingly.
