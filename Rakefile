# Rakefile for Jekyll site

desc "Install dependencies"
task :install do
  puts "Installing gem dependencies..."
  sh "bundle install"
end

desc "Run development server with live reload"
task :serve do
  puts "Starting Jekyll development server with live reload..."
  sh "bundle exec jekyll serve --livereload --baseurl '' --config _config.yml,_config_dev.yml"
end

task default: :serve
