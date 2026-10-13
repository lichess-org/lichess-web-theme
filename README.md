# @lichess/web-theme

Shared Lichess look: colors, type, and a few named classes.

Values are a high-level extract of lila’s dark/light themes (`ui/lib/css/theme`),
not a full port of the lichess.org stylesheet. Licensed under
[AGPL-3.0-or-later](./LICENSE).

## Plain HTML / static sites

```html
<link rel="stylesheet" href="./lichess.css" />
<button class="btn-primary">Submit</button>
```

`lichess.css` pulls in Noto Sans and Roboto from Google Fonts, then tokens and
named classes.

## Tailwind v4 apps

The Google Fonts `@import` must come first (CSS rule: imports before other
statements). Then Tailwind, then this package:

```css
@import url("https://fonts.googleapis.com/css2?family=Noto+Sans:ital,wght@0,400;0,500;0,600;0,700;1,400&family=Roboto:wght@300;400;500;700&display=swap");
@import "tailwindcss";
@import "@lichess/web-theme/tailwind.css";
@import "@lichess/web-theme/components.css";
```

Dark is the default. Light uses `html.light`.
