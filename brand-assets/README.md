# Brand assets (source, not published)

`logo-source.png` is the original Roadrunner Mission Lab logo file as
provided — full color, opaque white background. It's kept here for
provenance/future regeneration and is **not** copied into the built site
(it lives outside `src/_includes/img`, which is what gets published).

The processed assets actually used on the site live in
`src/_includes/img/brand/`:

- `logo.png` — full lockup (icon + wordmark), recolored for dark
  backgrounds (navy → cream, red and the compass/star accent kept as-is),
  transparent background. Used in the site header.
- `mark.png` — the icon only (bird + compass), same dark-background
  recolor, cropped tight with transparency. Used in the footer, the "Roadrunner
  Mission Lab" badge on the homepage, and as the source for the favicon /
  apple-touch-icon.

If a real vector (SVG) or a higher-resolution export of the logo becomes
available, swap it in here and regenerate `logo.png` / `mark.png` /
`favicon.png` / `apple-touch-icon.png` at higher fidelity — the current
versions were derived from a 493×131px screenshot, which is soft at large
sizes and very small favicon sizes.
