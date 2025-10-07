# tony-art.com — Starter

A lightweight, secure personal site for Tony. Static HTML, deployed on Vercel, DNS via Cloudflare.

## Quick Start
1. **Create repo** on GitHub and add these files.
2. **Deploy**: Import the repo into Vercel → Deploy.
3. **Domain**: In Vercel → Settings → Domains: add `tony-art.com` and `www.tony-art.com`. Set the apex as Primary and enable the redirect for `www`.
4. **DNS (Cloudflare)**:
   - `A` record: `tony-art.com` → `76.76.21.21`
   - `CNAME` record: `www` → `cname.vercel-dns.com`
   - Turn on: Always Use HTTPS, HSTS, and DNSSEC (recommended).
5. **Contact form**: Replace the Formspree endpoint in `index.html`.
6. **Email**: Optionally set Cloudflare Email Routing for `hello@tony-art.com` → your Gmail.
7. **Analytics**: Add Plausible or Umami script if desired.

## Customize
- Replace LinkedIn/GitHub URLs in `index.html`.
- Put your `/assets/favicon.ico` and optional `/assets/headshot.jpg`.
- Add `resume.pdf` at the repo root (the nav link points to it). You can also keep `/resume` redirect.
- Update `sitemap.xml` `lastmod` if you change pages.

## Security
- `vercel.json` sets strong headers (CSP, HSTS, etc.). If you add external scripts, update CSP.

## Local Preview
Just open `index.html` in a browser. Since it's static, no build step required.
