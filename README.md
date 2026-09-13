# Roadrunner Mission Lab

A public-facing microsite introducing **Roadrunner Mission Lab** — Roadrunner
Food Bank of New Mexico's innovation and earned-revenue initiative — to
funders, health-system partners, researchers, and anyone else who wants to
understand what it is and how to get involved.

Adapted from two internal source documents (an August 2026 board update and
a working-draft capital-strategy deck) and rewritten for an external
audience — no internal-only framing (board-meeting language, distribution
notices, asks addressed to a specific consulting program):

- The homepage tells the Mission Lab story, with the **Four Lanes** (Food Is
  Medicine, Research + Data Sharing, Waste-to-Value Solutions, Cold Chain +
  Local Agriculture) as the centerpiece.
- [`/strategy/`](src/strategy.njk) ("How It Works") covers who RRFB is, why
  this initiative exists, the five program areas, how opportunities get
  chosen, early traction, the 3-year roadmap, and how to partner with us.

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
| `src/_data/board.json` | Homepage content |
| `src/_data/strategy.json` | "How It Works" page content (`/strategy/`) |
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
