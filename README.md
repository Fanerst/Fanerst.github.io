# Feng Pan Academic Website

Personal and research-group website for Feng Pan, Assistant Professor in the
Science, Mathematics and Technology Cluster at SUTD.

This site is based on
[sbryngelson/academic-website-template](https://github.com/sbryngelson/academic-website-template),
a Jekyll template for academic and research group websites.

## Local Preview

```bash
bundle install
bundle exec jekyll serve
```

Then open <http://127.0.0.1:4000/>.

For live reload while editing:

```bash
bundle exec jekyll serve --livereload
```

For a one-time build:

```bash
bundle exec jekyll build
```

## Editing

- Site identity, navigation, links, and theme color: `_config.yml`
- Homepage text: `_pages/home.md`
- Research areas: `_pages/research.md`
- Open positions: `_pages/positions.md`
- News: `_data/news.yml` (up to 20 appear on the home page; all appear at `/news/`)
- Talks: `_data/talks.yml`
- Service: `_data/service.yml`
- Publications: `assets/ref.bib`
- CV: `papers/cv.pdf`
- Profile image: `images/feng-pan.jpg`

## Deployment

The repository includes `.github/workflows/deploy.yml`, which builds the Jekyll
site and deploys it to GitHub Pages using GitHub Actions. In the GitHub
repository settings, configure Pages to use GitHub Actions as the publishing
source.
