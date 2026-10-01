# portfodavid

Personal site for David Sunday David — published at
https://soyaya.github.io/portfodavid/ via GitHub Pages.

## What this is

A deliberately plain static HTML page (no build step, no framework) so it's
fast and fully readable by search crawlers without executing JavaScript for
the core content. The only JS on the page progressively enhances one small
widget (live GitHub stats) and does nothing the page needs to be readable.

## Files

- `index.html` — the whole site.
- `PERSONAL-FACTS.md` — the single source of truth every claim on the page
  is grounded in. Update this first, then update `index.html` to match.
  Anything not in this file shouldn't be on the page.
- `data/stats.json` — GitHub repo/follower/star counts, refreshed daily by
  `.github/workflows/update-stats.yml` (public GitHub API, no auth needed).
  Everything else on the page (AutoRamp transactions, Udemy enrollment,
  etc.) is a dated static figure, not live — those platforms have no public
  API this site can safely poll.
- `robots.txt`, `sitemap.xml` — basic crawl/indexing hygiene.

## Setup still needed

1. Enable GitHub Pages: repo Settings → Pages → Source: `Deploy from a
   branch` → Branch: `main` / `(root)`.
2. Submit the URL to Google Search Console and request indexing (this is
   what actually gets it appearing in search within days, not weeks).
3. Add the real Udemy course URL in `index.html` (currently a TODO) once
   confirmed.
4. Link back to this site from LinkedIn, GitHub profile README and any
   other profile you keep - consistent cross-linking between a handful of
   real, complete profiles is what Google's name-search ranking actually
   weighs, not volume.
