# TIRI — Personal Blog Theme

A minimal, editorial personal blog theme built with pure HTML, CSS, and vanilla JavaScript. No frameworks, no build step — just drop it in and go.

## Features

- **Zero dependencies** — no npm, no bundler, no framework
- **Editorial minimalism** — stark white background, all black text, Cormorant Garamond serif headings
- **Hero banner integration** — full-viewport hero with your banner image
- **Scroll-driven nav** — transparent over hero, white + border after scroll
- **Intersection Observer reveals** — staggered fade-in on scroll
- **Fully responsive** — adapts to mobile, tablet, and desktop
- **GitHub Pages ready** — deploy in one click

## Structure

```
/
├── index.html          ← Main blog page
├── TIRI_UK_BANNER_2026.png  ← Hero + featured image
└── README.md
```

## Deploying to GitHub Pages

1. Push this folder to a new GitHub repository
2. Go to **Settings → Pages**
3. Set source to `main` branch, root folder
4. Your site will be live at `https://yourusername.github.io/repo-name`

## Customisation

All design tokens are CSS variables at the top of the `<style>` block:

```css
:root {
  --white: #ffffff;
  --black: #000000;
  --serif: 'Cormorant Garamond', serif;
  --mono: 'Geist Mono', monospace;
  --sans: 'Geist', sans-serif;
}
```

Replace post content, author bio, and social links directly in the HTML — it's all clearly commented and sectioned.

## Fonts

Loaded from Google Fonts (no download needed):
- **Cormorant Garamond** — display headings
- **Geist** — body text
- **Geist Mono** — labels, metadata, UI chrome

---

© 2026 TIRI
