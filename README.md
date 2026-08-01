# Portfolio site (Quarto)

## Local setup
1. Install Quarto: https://quarto.org/docs/get-started/ (or `brew install quarto` / download from GitHub releases)
2. From this folder: `quarto preview` — opens a live-reloading local server.
3. `quarto render` — builds the static site into `_site/`.

## Publishing (free options)
- **GitHub Pages**: push this repo to GitHub, then `quarto publish gh-pages` from this folder — it builds and pushes `_site/` to a `gh-pages` branch automatically.
- **Netlify**: connect the repo, build command `quarto render`, publish directory `_site`.

## Structure
- `index.qmd` — landing page
- `projects.qmd` — portfolio / shipped artifacts page
- `blog.qmd` — auto-generated listing of everything in `posts/`
- `posts/<slug>/index.qmd` — one folder per blog post (keeps images/assets alongside the post)
- `about.qmd` — bio
- `_quarto.yml` — site config, nav bar
- `styles.css` — custom CSS overrides

## To do before publishing
- [ ] Add real email / GitHub / LinkedIn links (index.qmd, _quarto.yml navbar icons)
- [ ] Add repo/demo links in projects.qmd
- [ ] Replace placeholder post in posts/2026-07-quarto-site-launch/ with a real writeup
- [ ] Link resume PDF from about.qmd
- [ ] Pick a custom domain or use the default *.github.io / *.netlify.app URL
