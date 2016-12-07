source 'https://rubygems.org'

gemspec

gem 'inflecto'

gem 'rom-support', git: 'https://github.com/rom-rb/rom-support.git'
gem 'rom', git: 'https://github.com/rom-rb/rom.git'

group :development, :test do
  gem 'rom-sql', '~> 0.8', git: 'https://github.com/rom-rb/rom-sql.git'
end

group :development do
  gem 'dry-equalizer', '~> 0.2'
  gem 'sqlite3', platforms: [:mri, :rbx]
  gem 'jdbc-sqlite3', platforms: :jruby
end

group :test do
  gem 'rspec'
  gem 'dry-struct'
  gem 'byebug', platforms: :mri
  gem 'pg', platforms: [:mri, :rbx]
  gem 'jdbc-postgres', platforms: :jruby

  platform :mri do
    gem 'codeclimate-test-reporter', require: false
    gem 'simplecov'
  end
end

group :benchmarks do
  gem 'hotch', platforms: :mri
  gem 'benchmark-ips'
  gem 'activerecord', '~> 4.2'
end

group :tools do
  gem 'pry'
end
