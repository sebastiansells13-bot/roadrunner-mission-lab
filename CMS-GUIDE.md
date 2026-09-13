# Editing this site's content

You can update everything on this site — the board update, the four lanes,
the full strategy report — without touching any code.

## 1. Log in

1. Go to `https://app.pagescms.org/edit/sebastiansells13-bot/roadrunner-mission-lab`
2. Sign in with GitHub and authorize Pages CMS the first time you visit.

## 2. What you can edit

- **Site Settings** — site name, tagline, top navigation links.
- **Board Update (Culture of Possibility Realized)** — the homepage story: the
  hero, the track-record stat, the "why now" stat, the four case studies, the
  **Four Lanes** (Food Is Medicine, Research + Data Sharing, Waste-to-Value,
  Cold Chain + Local Agriculture — each with its own figure and color), the
  "where this leads" diagram, and the closing statement.
- **Full Strategy Report** — every section of the `/strategy/` page: who RRFB
  is, why now, the operating portfolio, the vetting criteria and near-term
  decisions, proof points, the 3-year roadmap, and where help is needed.

## 3. Making a change

1. Click into a content group (e.g. "Board Update")
2. Open a section (e.g. "Four Lanes") and edit the fields — required fields
   are marked
3. For a repeating list (lanes, case studies, proof points, etc.), click
   **Add** to create a new item, drag to reorder, or the trash icon to remove
   one
4. Click **Save**

Saving commits directly to the `main` branch, which triggers GitHub Actions to
rebuild and redeploy the site. It typically takes 1–3 minutes for changes to
go live — refresh the page after a few minutes if you don't see them right
away. You can watch progress under the repo's **Actions** tab.

## 4. Tips

- Keep the four lanes' **Accent color** values as `crimson`, `azure`, `sage`,
  or `teal` — those map to the site's color system.
- Icons for the four lanes are limited to `pulse`, `scan`, `leaf`, and
  `snowflake` by design, to keep the visual language consistent.
- If something looks wrong after publishing, check the Actions tab for a
  failed build before re-editing — most issues are a missing required field.
