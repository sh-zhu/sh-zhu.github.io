# sh-zhu.github.io

A minimal, single-page academic homepage. Built on Jekyll + [jekyll-scholar](https://github.com/inukshuk/jekyll-scholar)
(kept for bibtex-driven publications), everything else hand-written — no
Bootstrap/jQuery, no build framework, a few KB of CSS.

## Fill in your content

- **About** — edit `_pages/about.md`: bio paragraph, title/affiliation, and
  swap `assets/img/prof_pic.jpg` for your real photo.
- **Social links** — edit `_data/socials.yml` (uncomment the keys you want:
  email, github_username, scholar_userid, etc.).
- **News** — add one file per item in `_news/` (copy `announcement_1.md`).
  `inline: true` renders as a one-liner; `inline: false` renders a full post.
- **Publications** — add one BibTeX entry per paper to
  `_bibliography/papers.bib`. See the comment at the top of that file for
  supported fields (`abbr`, `pdf`, `arxiv`, `code`, `html`, `doi`).
- **Service** — add one entry per role to `_data/service.yml`.
- **Analytics** (optional) — create a free account at
  [goatcounter.com](https://www.goatcounter.com/) and set `goatcounter_id` in
  `_config.yml`.

## Adding a page later

Add a new file to `_pages/` with `layout: minimal` in its front matter, then
add a link to it in the top nav in `_layouts/minimal.liquid`. No other
changes needed.

## Local development

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.

## Deploy

Pushing to `main` triggers `.github/workflows/deploy.yml`, which builds the
site and publishes it to GitHub Pages.

## Acknowledgements

This site is adapted from [al-folio](https://github.com/alshedivat/al-folio) by
Maruan Al-Shedivat and contributors, released under the MIT License. The
original copyright notice is kept in [LICENSE](LICENSE).
