# frozen_string_literal: true

source "https://rubygems.org"

gemspec
rails_version = "#{ENV['RAILS_VERSION'] || '6.0.3.2'}"

gem "rake", "~> 12.0"
# Bundle edge Rails instead: gem 'rails', github: 'rails/rails'
gem "rails", rails_version == "master" ? { github: "rails/rails" } : rails_version
# Use Puma as the app server
gem "puma", "~> 4.1"
# Transpile app-like JavaScript. Read more: https://github.com/rails/webpacker
gem "webpacker", "~> 5.0"

# Reduces boot times through caching; required in config/boot.rb
gem "bootsnap", ">= 1.4.2", require: false

group :development, :test do
  # Call 'byebug' anywhere in the code to stop execution and get a debugger console
  gem "minitest", "~> 5.0"
  gem "pry-rails"
end

group :development do
  # Spring speeds up development by keeping your application running in the background. Read more: https://github.com/rails/spring
  gem "spring"
  gem "spring-watcher-listen", "~> 2.0.0"
end

group :test do
  # Adds support for Capybara system testing and selenium driver
  gem "capybara", "~> 3"
end
