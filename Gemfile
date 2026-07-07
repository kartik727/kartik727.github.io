source "https://rubygems.org"

# This site runs on Jekyll 4 and is deployed via GitHub Actions
# (see .github/workflows/deploy.yml), so it no longer depends on the
# github-pages gem / legacy branch builder. Run locally with:
#
#     bundle install
#     bundle exec jekyll serve --livereload
#
gem "jekyll", "~> 4.3"

# Plugins
group :jekyll_plugins do
  gem "jekyll-feed"
  gem "jekyll-sitemap"
  gem "jekyll-gist"
  gem "jekyll-redirect-from"
  gem "jemoji"
end

# Windows and JRuby do not include zoneinfo files, so bundle the tzinfo-data gem
# and associated library.
gem "tzinfo-data", platforms: [:mingw, :mswin, :x64_mingw, :jruby]
gem "wdm", "~> 0.1.0", platforms: [:mingw, :mswin, :x64_mingw]

gem "webrick", "~> 1.8"
