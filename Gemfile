source "https://rubygems.org"

# Core Jekyll engine
gem "jekyll", "~> 4.4.1"
gem "minima", "~> 2.5"

# Chirpy uses remote theme, so no need to include a local theme gem

# Plugins
group :jekyll_plugins do
 
  gem "jekyll-feed"  # Add this if not present
 
end

# Windows and JRuby support (optional)
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end

gem "wdm", "~> 0.1", :platforms => [:mingw, :x64_mingw, :mswin]
gem "http_parser.rb", "~> 0.6.0", :platforms => [:jruby]
