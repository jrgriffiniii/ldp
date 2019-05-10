source 'https://rubygems.org'

# Specify your gem's dependencies in ldp-client.gemspec
gemspec

gem 'slop', '~> 3.6' if RUBY_PLATFORM == "java"
gem 'byebug', platforms: [:mri]
gem 'activesupport'
gem 'capybara_discoball', '~> 0.0.2'
gem 'derby',              '~> 0.1.0'

if ENV['RAILS_VERSION']
  if ENV['RAILS_VERSION'] == 'edge'
    gem 'rails', github: 'rails/rails'
  else
    gem 'rails', ENV['RAILS_VERSION']
  end
end

case ENV['RAILS_VERSION']
when /^5.1/
  gem 'rack', '~> 1.6'
end
