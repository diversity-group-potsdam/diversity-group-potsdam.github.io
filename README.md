# Research Group Website Template

A plain HTML/CSS/JS site — no build step, no dependencies. Open `index.html`
directly in a browser, or host it anywhere that serves static files.

## Structure

```
index.html      All page content (single page, anchor-linked sections)
css/style.css   Styling, incl. dark-mode support
js/main.js      Mobile nav toggle + footer year
assets/img/     Put photos/logos here
```

## Customize

Everything is in `index.html`, edited in place:

- **Lab name / university / colors** — swap the text, and update
  `--color-accent` at the top of `css/style.css`.
- **People** — duplicate a `.person-card` block under `#people`. Replace the
  `<div class="avatar">JD</div>` initials with `<img src="assets/img/name.jpg" alt="...">`
  once you have real photos.
- **Publications** — duplicate an `<li>` under `#publications`, grouped by
  `<h3 class="group-label">Year</h3>`.
- **News** — add `<li>` entries under `#news`, newest first.

## Deploy

Simplest option is GitHub Pages:

```bash
git init
git add .
git commit -m "Initial site"
git branch -M main
git remote add origin <your-repo-url>
git push -u origin main
```

Then enable Pages for the repo (Settings → Pages → Deploy from branch → `main`).
Any static host (Netlify, Vercel, university web space) works the same way —
just upload the folder.
