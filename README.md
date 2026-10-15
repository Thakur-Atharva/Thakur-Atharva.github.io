# Atharva Thakur — personal site

Single-page static site (`index.html`, no build step), deployed to GitHub Pages by
`.github/workflows/deploy.yml` on every push to `main`.

- Edit `index.html`; colors/fonts are the `:root` tokens at the top of its `<style>`.
- Optional files published next to it: `resume.pdf`, and an `assets/` folder for images.
  To show the CV link, add `resume.pdf` and a `<a href="resume.pdf">CV</a>` in the sidebar.
- `site-options/` holds alternative designs (not published). See its README to switch.
