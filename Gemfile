source 'https://rubygems.org'

group :development, :test do
  gem 'puppetlabs_spec_helper', :require => false
  gem 'rspec-system-puppet', '~>2.0'
  gem 'puppet-lint'
  gem 'puppet-blacksmith',  '> 3.0'
  gem 'metadata-json-lint'
  if RUBY_VERSION < "2.0.0"
    gem 'json', '< 2.0' # newer versions requires at least ruby 2.0
  end
end

if puppetversion = ENV['PUPPET_GEM_VERSION']
  gem 'puppet', puppetversion, :require => false
else
  gem 'puppet', :require => false
end
