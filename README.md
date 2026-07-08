# Usami Rika Dojo

Website for **Usami Rika Dojo** (宇佐美Rika道場) — the karate dojo of 2012 World
Kata Champion Rika Usami in Iwami, Tottori, Japan.

**Live site:** https://gordonjaychan1.github.io/UsamiRikaDojo/

## About

A single-page, fully self-contained site. All styles and scripts are inline in
`index.html` — there is no build step and no runtime dependencies. Every asset
is hosted in this repo (no external image CDNs).

Features:

- **Bilingual** English / Japanese, toggled in the nav and remembered via
  `localStorage`.
- Hand-rolled vanilla JS for the loading screen, scroll reveals, parallax hero,
  gallery lightbox, blog expand/collapse, and language switching.
- Responsive down to phones, with `prefers-reduced-motion` support.
- SEO/social metadata (Open Graph, Twitter cards, JSON-LD structured data).

## Structure

```
.
├── index.html      # The entire site — markup, CSS, and JS
├── favicon.svg     # Site icon (kept at repo root by convention)
├── images/         # All photos and graphics
│   ├── hero.jpg
│   ├── about-champion.jpg
│   ├── gallery-1.jpg … gallery-7.jpg
│   ├── group-lessons.jpg
│   ├── private-lessons.jpg
│   ├── seminars.jpg
│   ├── flyer.jpg
│   └── usamidojo.avif
└── README.md
```

## Editing content

- **Text / translations** live inline in `index.html`. Most elements carry
  `data-en` / `data-jp` attributes; longer passages use `.bilingual` blocks with
  `.lang-en` / `.lang-jp` children.
- **Blog posts** are the JSON array in the `<script id="blog-data">` block near
  the bottom of `index.html`. Add an object with `slug`, `date_en`, `date_jp`,
  `title_en`, `title_jp`, `image`, `body_en`, `body_jp`.
- **Images** go in `images/`. Reference them with a relative path
  (`images/your-file.jpg`); the Open Graph / Twitter / JSON-LD tags need the
  **absolute** GitHub Pages URL.

## Local preview

No build required — open `index.html` in a browser, or serve the folder:

```sh
python -m http.server 8000   # then visit http://localhost:8000
```

## Deployment

Hosted on **GitHub Pages** from the `main` branch. Pushing to `main`
automatically rebuilds and publishes the live site within a minute or so.
