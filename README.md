# Lichess Web Theme

This repo contains Lichess styles that can be used by other websites and apps.

Styling was extracted from lila’s dark/light themes (`ui/lib/css/theme`), but it
is not 100% accurate or complete. It's a good starting point for getting a
website closer to the appearance of Lichess.org.

## Plain HTML / static site usage

```html
<link
  rel="stylesheet"
  href="https://cdn.jsdelivr.net/gh/lichess-org/lichess-web-theme@main/lichess.css"
/>
<button class="btn-primary">Submit</button>
```

## Tailwind app usage

The Google Fonts `@import` must come first, then Tailwind, then this package:

```css
@import url("https://fonts.googleapis.com/css2?family=Noto+Sans:ital,wght@0,400;0,500;0,600;0,700;1,400&family=Roboto:wght@300;400;500;700&display=swap");
@import "tailwindcss";
@import "lichess-web-theme/tailwind.css";
@import "lichess-web-theme/components.css";
```
