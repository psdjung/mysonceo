# My Son CEO

The site for **My Son CEO**, built on the [Chirpy][chirpy] Jekyll theme (same setup as [peterjung.site][peterjung-site]).

## Local development

```bash
bundle install
bundle exec jekyll serve --livereload
```

Site will be available at `http://127.0.0.1:4000`.

## Structure

- `_config.yml` — site title, tagline, social links, feature toggles
- `_tabs/about.md` — the About page content
- `_data/authors.yml` — post author metadata
- `_posts/` — blog posts (add new posts here as `YYYY-MM-DD-title.md`)
- `assets/img/personal/` — add a logo/avatar here and point `avatar:` in `_config.yml` at it

## Deployment

Pushes to `main` build and deploy via the GitHub Actions workflow in
`.github/workflows/pages-deploy.yml`, publishing to GitHub Pages. The `CNAME`
file points the custom domain (`mysonceo.com`) at this repo — configure the
matching DNS record and enable the custom domain under the repo's
**Settings → Pages**.

[chirpy]: https://github.com/cotes2020/jekyll-theme-chirpy
[peterjung-site]: https://github.com/psdjung/peterjung-site
