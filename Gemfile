source "https://rubygems.org"

gemspec

gem 'pry-rails'
gem 'pry-nav'

gem 'localeapp'

platforms :jruby do
  gem "activerecord-jdbc-adapter", :require => false
end

group :test do
  platforms :ruby do
    gem "forem-redcarpet"
    gem "mysql2"
    gem "sqlite3"
  end

  platforms :jruby do
    gem "activerecord-jdbcmysql-adapter", :require => false
    gem "activerecord-jdbcpostgresql-adapter", :require => false
    gem "activerecord-jdbcsqlite3-adapter", :require => false
    gem "forem-kramdown"
  end
end

if RUBY_VERSION < '1.9.2'
  gem 'nokogiri', '~> 1.5.9'
end
