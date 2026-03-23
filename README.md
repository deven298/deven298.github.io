# deven298.github.io

Personal portfolio site, live at [deven298.github.io](https://deven298.github.io).

Built with plain HTML/CSS/JS and served via GitHub Pages.

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

## Deploying

Push to `main` — GitHub Pages auto-builds and deploys within ~30 seconds.

```bash
git add .
git commit -m "your message"
git push origin main
```

No CI, no build pipeline needed.