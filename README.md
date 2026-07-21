# yoonbai.github.io — personal research site

A small multi-page static site. No build step. Shared styling lives in `static/site.css`;
figures/GIFs/videos go in `static/media/`.

## Pages
- `index.html` — intro + gateway to the research topics (this is your home page)
- `3d-surface.html` — Cortex · 3D surface estimation in the brain (bioRxiv)
- `straightening.html` — Representation · straightening & predictive coding
- `vr-grasping.html` — Behavior · VR psychophysics of grasping (filled from your deck + progress report)

## Host on GitHub Pages
1. Create a repo named exactly **`yoonbai.github.io`**.
2. Put every file here at the repo root, keeping the `static/` folder intact.
3. Push. In **Settings → Pages**, confirm the source is `main` / root.
4. Live at **https://yoonbai.github.io**.

Local preview: `python3 -m http.server` then open http://localhost:8000

## Extending it (built to scale)
- **New research topic** → copy a topic page (e.g. `3d-surface.html`) to `newtopic.html`,
  copy one `<a class="gate-card">` on `index.html` to point at it, and add a nav link.
- **New publication** → copy one `<li class="pub">`.
- **New figure/GIF/MP4** → drop the file in `static/media/` and replace a `.media-frame`
  placeholder. Each frame has a commented-in `<img>` / `<video>` example and the expected filename.
- **Style once, everywhere** → edit `static/site.css`; every page updates.

## Placeholders to fill (highlighted red on the page = `<span class="fill">`)
- Exact bioRxiv title / authors / headline result
- Your straightening (PhD) publication details
- VR page: your measured tracking SDs, the stain-pinch pilot error figure, and your role on the project

## Notes
- Nav uses **Cortex · Representation · Behavior** — the three levels of your program — rather than generic 01/02/03.
- The VR page credits **Weiwen Tian** as project lead; your role is a `fill` for you to set.
- ReStraV (arXiv:2507.00583, NeurIPS 2025) is shown as a *downstream application* of your straightening framework, never as your own paper.
- Specific unpublished numbers on the VR page are left as `fill` placeholders so you decide what to disclose.
