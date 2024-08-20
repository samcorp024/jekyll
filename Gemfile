source "https://rubygems.org"

# Specify the version of Jekyll
gem "jekyll", "~> 4.3.3"

# Default theme for Jekyll
gem "minima", "~> 2.5"

# Uncomment the line below if using GitHub Pages and comment out the Jekyll gem line above
# gem "github-pages", group: :jekyll_plugins

# Jekyll plugins
group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.12"
end

# tzinfo-data gem for Windows and JRuby
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

# Update wdm to the version installed on your system
gem "wdm", "~> 0.2.0", platforms: [:mingw, :x64_mingw, :mswin]

# Lock http_parser.rb version on JRuby
gem "http_parser.rb", "~> 0.6.0", platforms: [:jruby]
