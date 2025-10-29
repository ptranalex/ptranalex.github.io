source "https://rubygems.org"

# Jekyll
gem "jekyll", "~> 4.3"

# Chirpy theme
gem "jekyll-theme-chirpy", "~> 7.1"

# Jekyll plugins
group :jekyll_plugins do
  gem "jekyll-feed"
  gem "jekyll-sitemap"
  gem "jekyll-seo-tag"
  gem "jekyll-archives"
  gem "jekyll-paginate"
end

# Add webrick for Ruby 3.0+
gem "webrick", "~> 1.7"

# Performance booster for file watching on macOS/Windows
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
  gem "wdm", "~> 0.1.1"
end