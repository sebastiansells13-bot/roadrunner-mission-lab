# Roadrunner Mission Lab

A microsite for Roadrunner Food Bank of New Mexico's innovation and
earned-revenue initiative — **Roadrunner Mission Lab**.

Built from two source documents:

- *Culture of Possibility, Realized* (board update, August 2026) — the
  homepage narrative, with the **Four Lanes** (slide 5 — Food Is Medicine,
  Research + Data Sharing, Waste-to-Value Solutions, Cold Chain + Local
  Agriculture) as the centerpiece.
- *Innovation & Earned Revenue: Capital Strategy* (working draft, August
  2026) — reproduced in full on the [`/strategy/`](src/strategy.njk) page:
  who RRFB is, why now, the current operating portfolio, the vetting
  process, proof points, the 3-year roadmap, and where outside help is
  needed.

Eleventy (11ty) + Nunjucks + Sass, content editable through [Pages
CMS](https://pagescms.org) (see [CMS-GUIDE.md](CMS-GUIDE.md)), deployed to
GitHub Pages via GitHub Actions.

## Design

Deliberately not the [client-site-starter](https://github.com/sebastiansells13-bot/client-site-starter)
look: a dark, editorial palette (desert navy, crimson, and gold, pulled from
RRFB's own brand marks) with Fraunces/Inter/IBM Plex Mono typography, in
place of the starter's white background and system fonts.

## Quick start

```bash
npm install
npm start
```

Visit http://localhost:8080/.

## Structure

| File/dir | Purpose |
|---|---|
| `.pages.yml` | Pages CMS content model |
| `src/_data/site.json` | Site name, tagline, navigation |
| `src/_data/board.json` | Board-update content (homepage) |
| `src/_data/strategy.json` | Full strategy report content (`/strategy/`) |
| `src/_includes/css/` | Design tokens + styles (Sass) |
| `.github/workflows/build-deploy.yml` | CI: build + deploy to GitHub Pages |
| `CMS-GUIDE.md` | Content-editor walkthrough |

## Deploy

Push to `main` — GitHub Actions builds the site and publishes it to GitHub
Pages automatically. Enable Pages once under **Settings → Pages → Source:
GitHub Actions**.

## Content editing

See [CMS-GUIDE.md](CMS-GUIDE.md). Editors sign in at
`https://app.pagescms.org/edit/sebastiansells13-bot/roadrunner-mission-lab`
with GitHub — no server, no separate login system.

## License

Internal project for Roadrunner Food Bank of New Mexico — not licensed for
redistribution.
