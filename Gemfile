source "https://rubygems.org"
git_source(:github) { |repo| "https://github.com/#{repo}.git" }

ruby "~> 3.2"

gem "aws-sdk-s3", require: false
gem "bootsnap", require: false # Reduces boot times through caching; required in config/boot.rb
gem "cssbundling-rails"
gem "devise"
gem "devise-jwt"
gem "haml"
gem "image_processing", "~> 1.2"
gem "jbuilder"
gem "jsbundling-rails"
gem "jwt"
gem 'omniauth-github', '~> 2.0.0'
gem "omniauth-rails_csrf_protection"
gem "pg", "~> 1.1"
gem "puma", "~> 5.0"
gem "rack-cors"
gem 'rails', '~> 7.1', '>= 7.1.2'
gem "redis", "~> 5.0"
gem "sidekiq", "~> 7.0"
gem "sprockets-rails"
gem "stimulus-rails"
gem "turbo-rails"
gem "tzinfo-data", platforms: %i[mingw mswin x64_mingw jruby] # Windows does not include zoneinfo files, so bundle the tzinfo-data gem
gem "view_component"

# Use Redis adapter to run Action Cable in production
# gem "redis", "~> 4.0"

# Use Kredis to get higher-level data types in Redis [https://github.com/rails/kredis]
# gem "kredis"

# Use Active Model has_secure_password [https://guides.rubyonrails.org/active_model_basics.html#securepassword]
# gem "bcrypt", "~> 3.1.7"

# Use Sass to process CSS
# gem "sassc-rails"

group :development, :test do
  # See https://guides.rubyonrails.org/debugging_rails_applications.html#debugging-with-the-debug-gem
  gem "debug", platforms: %i[mri mingw x64_mingw]
  gem "factory_bot_rails", "~> 6.2"
  gem "rspec-rails", "~> 6.0"
end

group :development do
  # Use console on exceptions pages [https://github.com/rails/web-console]
  gem "web-console"
  # Add speed badges [https://github.com/MiniProfiler/rack-mini-profiler]
  # gem "rack-mini-profiler"

  gem "dockerfile-rails", "~> 1.2"
  gem "rubocop", "~> 1.44", require: false
  gem "rubocop-performance", "~> 1.15", require: false
  gem "rubocop-rails", "~> 2.17", require: false
  gem "rubocop-rspec", "~> 2.18", require: false
  gem "spring"
  gem "spring-commands-rspec"
end

group :test do
  gem "capybara"
  gem "cuprite"
  gem "faker"
end
