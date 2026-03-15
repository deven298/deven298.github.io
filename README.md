# deven298.github.io

Personal portfolio site, live at [deven298.github.io](https://deven298.github.io).

Built with plain HTML/CSS/JS and served via GitHub Pages. Jekyll is used only as the GitHub Pages build layer — there are no templates or Liquid tags; `index.html` and `404.html` are written directly.

---

## Project structure

```
.
├── index.html          # Main portfolio page
├── 404.html            # Custom 404 page
├── style.css           # All styles (design tokens, layout, components)
├── _config.yml         # Jekyll / GitHub Pages config
├── Gemfile             # Ruby deps (Jekyll + github-pages gem)
├── images/
│   └── favicon.ico     # Browser tab icon
└── assets/
    └── Deven_Resume.pdf      # Resume PDF for download
```

---

## Local dev

**Prerequisites:** Ruby ≥ 3.x and Bundler.

```bash
# 1. Install deps (first time only)
bundle install

# 2. Serve with live reload
bundle exec jekyll serve --livereload

# 3. Open in browser
open http://localhost:4000
```

> Since the site is plain HTML, you can also just open `index.html` directly in a browser with no build step — useful for quick edits.

---

## Making changes

| What | Where |
|---|---|
| Content (text, links, jobs) | `index.html` |
| All styling and layout | `style.css` |
| Design tokens (colors, fonts) | `:root` block at top of `style.css` |
| 404 page | `404.html` |
| Resume PDF | `assets/Deven_Resume.pdf` |

**Key CSS variables** (in `style.css`):
```css
--accent:  #00d4aa   /* teal — primary brand colour */
--accent2: #0088ff   /* blue — secondary accent */
--bg:      #080b10   /* page background */
--font-display: 'Syne'    /* headings */
--font-mono:    'DM Mono' /* labels, tags */
--font-body:    'DM Sans' /* body text */
```

---

## Deploying

Push to `main` — GitHub Pages auto-builds and deploys within ~30 seconds.

```bash
git add .
git commit -m "your message"
git push origin main
```

No CI, no build pipeline needed.

---

## Favicon

Place your favicon file in `images/` and make sure `index.html` and `404.html` both have this in `<head>`:

```html
<link rel="icon" type="image/x-icon" href="images/favicon.ico" />
<link rel="apple-touch-icon" href="images/favicon.ico" />
```