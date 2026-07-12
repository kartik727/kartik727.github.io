# kartikc727.github.io

Source for my personal website, [kartikc.com](https://kartikc.com).

## Stack

Built with [Jekyll](https://jekyllrb.com) and hosted on GitHub Pages. The theme is a
customized fork of [AcademicPages](https://github.com/academicpages/academicpages.github.io),
which is itself a fork of the [Minimal Mistakes](https://mademistakes.com/work/minimal-mistakes-jekyll-theme/)
theme (© Michael Rose, MIT License — see `LICENSE`).

## Layout

- `_config.yml` — site-wide configuration.
- `_data/navigation.yml` — top navigation bar.
- `_pages/` — standalone pages (about, CV, publications).
- `_publications/`, — content collections.
- `_layouts/`, `_includes/`, `_sass/` — theme templates and styles.
- `assets/`, `images/`, `files/` — CSS/JS, images, and downloadable files (e.g. resume).

## Running locally

Requires Ruby 3.3 with Bundler. This project uses `chruby` and `.ruby-version`
for local Ruby selection; avoid Apple's system Ruby (currently Ruby 2.6).

```bash
ruby-install ruby 3.3.11
cd /path/to/kartik727.github.io
gem install bundler
bundle install
bundle exec jekyll serve
```

The site is served at `http://localhost:4000` and rebuilds on file changes.
