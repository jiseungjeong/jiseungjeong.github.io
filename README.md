# jiseungjeong.com

Personal academic site for **Jiseung Jeong**. Layout adapted from
[Jon Barron's website](https://jonbarron.info/).

Static HTML + CSS, served directly by GitHub Pages (`.nojekyll`) at
[jiseungjeong.com](https://jiseungjeong.com).

## Local preview

```bash
python3 -m http.server 4000
# open http://localhost:4000
```

## Structure

```
.
├── index.html                # single-page layout
├── style.css                 # all styles
├── CNAME                     # custom domain
├── .nojekyll                 # bypass Jekyll on GitHub Pages
└── assets/
    ├── JiseungJeong-CV.pdf
    └── img/
        ├── favicons/
        ├── profile.jpg              # ← header photo (add this)
        ├── research/
        │   └── premover.png         # ← research thumbnail (add this)
        └── projects/
            ├── fused-dequant.png    # ← project thumbnails (add these)
            ├── quantshift.png
            ├── shadow-boxing.png
            └── yolokemon.png
```

Thumbnails degrade gracefully — if a file is missing, the placeholder text
`research figure` / `project figure` is shown instead of a broken image.

## Editing

- **Content** — edit `index.html` directly. Each section is a plain
  `<article class="entry">` block; copy one to add a new entry.
- **Colors, spacing, fonts** — see the `:root` block at the top of
  `style.css`.

## License

MIT — see [LICENSE](LICENSE).
