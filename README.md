# www.imarand.com — Head Ventures / Crew Install (AI-written)

This repo **is** the live site for **www.imarand.com**, served by GitHub Pages (user site, auto-published from `main`).

- Static only: plain HTML + one stylesheet. No build step, no analytics, no cookies, no backend. The only JavaScript on the site is the small inline prompt-builder on `paste.html` (works without it — the template is copyable as-is).
- `mark.png` is the Head Ventures mark (cream H, brass rule, near-black field); `favicon.png` is a tight crop of the same mark.
- Pages: `index.html` (offer, pricing, trust, FAQ), `how-it-works.html`, `faq.html` (the long FAQ), `guides/cursor-cloud-agent-cannot-read-github-issues.html`, `paste.html` (free Paste-the-Ticket prompt builder), `about.html`, `404.html`.
- The homepage leads with the buyer's pain (the cloud VM token often lacks issues scope, so tickets sit and the agent guesses); "we never touch main" is a guarantee further down, not the headline.
- Primary CTA is `orders@imarand.com`. The $99 Merge Crew pack checkout is a Stripe payment link and stays secondary.
- `sitemap.xml` + `robots.txt` cover the indexable pages.
- `CNAME` must stay `www.imarand.com`.

Site content and this README are AI-written, and the site says so. A human still merges every PR.
