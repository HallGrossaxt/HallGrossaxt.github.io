# Homepage

Source for the personal homepage at **https://hallgrossaxt.github.io/**.

A single-page, dependency-free static site (plain HTML + CSS) — a short welcome,
an intro to the work, and links to the public GitHub repositories.

## Files

| File | Purpose |
|------|---------|
| `index.html` | Page content (hero, about, project cards, footer) |
| `style.css`  | Styling — responsive, light/dark via `prefers-color-scheme` |

No build step, no frameworks. Open `index.html` in a browser to preview locally.

## Customizing

- **Display name / handle:** edit the `<h1>` and footer in `index.html`
  (currently shows `HallGrossaxt`).
- **Intro text:** the `#about` section in `index.html`.
- **Projects:** each repo is a `.card` block in the `#projects` section — copy a block
  to add one, or edit the link/description/language dot (`fortran` / `python`).
- **Colors:** the `:root` design tokens at the top of `style.css`.

## Deploying to GitHub Pages

This is meant to replace the test page in the `HallGrossaxt.github.io` repo
(GitHub Pages serves the default branch root). To publish:

```sh
# from this folder, pointed at the Pages repo
git add index.html style.css README.md
git commit -m "New homepage"
git push origin main      # or master, whichever the Pages repo uses
```

GitHub Pages picks up the change automatically; the site updates within a minute or two.
