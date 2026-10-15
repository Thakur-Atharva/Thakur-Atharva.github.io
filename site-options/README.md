# Site design options

Each folder is a complete, self-contained site (one `index.html`, no build step).
All four share the same content.

| Folder | Description |
|---|---|
| `a-editorial/` | Serif, paper-like, sticky sidebar |
| `a-editorial-dag/` | Same as A plus an interactive causal DAG under the intro |
| `b-bento/` | Modern card grid with a chessboard card |
| `c-causal-graph/` | Dark, monospace, full-screen causal DAG hero |

## Preview

    python3 -m http.server -d site-options     # then open http://localhost:8000

## Switch to a design

Copy the chosen folder's contents to the repo root (GitHub Pages serves the root
`index.html`) and add your `resume.pdf` next to it:

    cp site-options/a-editorial-dag/index.html index.html

Because each design is a single file, switching later is just copying a different
`index.html` over the top. Content (bio, experience, links) is duplicated in each
file, so after you pick one, edit that copy and treat the others as archived.

## Where to customize

- Colors and fonts: the `:root { --... }` tokens at the top of each file's `<style>`.
- Graph shape (A+DAG, C): the `LAYERS` array in the `<script>`.
- Paper placeholder: search for "coming soon" and replace the title, authors and links.
- Photos / projects: replace the placeholder `.gallery` / `.photos` blocks with `<img>` tags.
