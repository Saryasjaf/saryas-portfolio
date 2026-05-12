# Saryas Jaf — Portfolio

Personal portfolio site for **Saryas Jaf** — Computer Engineer in Erbil, Kurdistan Region of Iraq. IT infrastructure, security systems, IoT solutions, and custom electronics.

**Live site:** https://saryasjaf.github.io/saryas-portfolio/

## Highlights

- **Dark cinematic design** — warm-gold accents on near-black palette
- **Trilingual** — English, العربية (Arabic), کوردی (Kurdish Sorani) with full RTL support
- **Fully responsive** — fluid `clamp()` scaling from small phones up to wide desktops; tablet and small-mobile breakpoints
- **Single-file architecture** — all HTML, CSS, and JavaScript in one file. No build step, no framework, no dependencies beyond Google Fonts.
- **Animated hero** — particle field, fade-up reveals, headline word-by-word entrance
- **Always-visible marquee** of skills/services at the viewport bottom
- **Working contact form** wired to Formspree with AJAX submission and trilingual success/error states
- **Accessibility** — `aria-*` attributes, keyboard nav, reduced-motion respect, 44×44 minimum tap targets

## Built with

- Plain HTML, CSS, vanilla JavaScript — no build step
- [Fraunces](https://fonts.google.com/specimen/Fraunces) (display italic) + [Inter](https://fonts.google.com/specimen/Inter) (body) + [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono) (metadata) + [IBM Plex Sans Arabic](https://fonts.google.com/specimen/IBM+Plex+Sans+Arabic) (AR/KU)
- [Formspree](https://formspree.io) — contact form backend
- Hosted on [GitHub Pages](https://pages.github.com)

## Run locally

The site is a single static HTML file. Two ways to preview:

**Direct file open** — double-click `index.html`, opens in your default browser.

**Local server** (recommended for mobile testing on real devices over Wi-Fi):

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000` (or `http://<your-IP>:8000` from a phone on the same Wi-Fi).

## File structure

```
saryas-site/
├── index.html                     ← Single-file site (HTML + inline CSS + inline JS)
├── README.md
├── .gitignore
└── assets/
    ├── favicon.ico
    ├── favicon.svg
    └── img/
        ├── logo-animated-light.svg          ← Brand logo (navbar)
        ├── hero-bg.png                       ← Hero photo (LTR desktop)
        ├── hero-bg-rtl.png                   ← Hero photo (RTL desktop, pre-mirrored)
        ├── hero-bg-mobile.jpg                ← Hero photo (LTR mobile, 2:3 portrait)
        ├── hero-bg-mobile-rtl.jpg            ← Hero photo (RTL mobile, pre-mirrored)
        ├── portrait-saryas.jpg               ← About section portrait
        ├── work-it-operations.jpg            ← Case study 1 photo
        ├── work-industrial-security.jpg      ← Case study 2 photo
        └── work-hardware-support.jpg         ← Case study 3 photo
```

## Editing

All content lives in `index.html`:

- **Text** in any language — search for the section by its English text and update the matching `data-en` / `data-ar` / `data-ku` attribute. The JS swaps `innerHTML` based on the active language.
- **Colors** — CSS variables at the top of the `<style>` block (`--bg`, `--gold`, `--gold-bright`, `--copper`, `--cream`, etc.)
- **Layout** — sections are marked with clear HTML comments (`§01 HERO`, `§02 PRACTICE`, etc.)
- **Photos** — replace files in `assets/img/` (keep filenames the same, or update the CSS `background-image` URLs and `<img src>` references)

## License

Personal content © 2026 Saryas Jaf.
