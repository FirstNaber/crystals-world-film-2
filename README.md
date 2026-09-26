# Crystals World — scroll-film edition, variation 2 ("The Specimen Room")

The film plays in the dark with a specimen label that rewrites itself per chapter (Amethyst, Clear quartz, Citrine);
below it, the shop is a lit room: warm paper, ink, museum-style captions. Plain HTML/CSS/JS, no build step.

- `site/index.html` — the whole page.
- `site/frames/x/` — 361 frames at 3200px, from the 4K upscale. Served to large screens (ultrawide, 4K, big retina).
- `site/frames/d/` — 361 frames at 1920px. Served to laptops and phones.
- In both sets, frames 104–172 are re-graded locally: the white flare between amethyst and quartz is replaced
  by a soft glow dissolve (peak brightness 191 → 86).
- `site/img/` — the shop's own photos.
- `src/` (local only) — the source video and its 4K upscale.

Run locally: `cd site && python3 -m http.server 8000`. Deploy: `./deploy.sh`.
