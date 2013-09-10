# Additional libraries are loaded in "config/initializers/libraries.rb".

# Repository:
source "https://rubygems.org"

# Rake version
gem 'rake', '~> 0.8.7'

# Rails version, which must be specified here AND in the environment.rb:
gem 'rails', '~> 3.2.0'

# Selectively-loaded:
gem 'facets',       '~> 2.8.0', :require => false # For initializers/dependencies.rb
gem 'mysql',        '~> 2.8.0', :require => false # For commonly used database driver
gem 'right_aws',    '~> 1.0',   :require => false # For paperclip
gem 'ruby-openid',  '~> 2.1.0', :require => false # For open_id_authentication
gem 'rack-openid',  '~> 1.3.1', :require => false # For open_id_authentication
gem 'sqlite3-ruby', '~> 1.2.0', :require => false # For default database driver
gem 'rwikibot',     '= 2.0.6',  :require => false,
                                :git => 'git://github.com/reidab/rwikibot.git'

# Necessary:
gem 'RedCloth',            '~> 4.2.3'
gem 'aasm'
gem 'acts-as-taggable-on'
gem 'color'
gem 'comma',               '~> 3.0'
gem 'fastercsv',           '~> 1.5.3'
gem 'gchartrb',            '~> 0.8.0', :require => 'google_chart'
gem 'hpricot',             '~> 0.8.2'
gem 'paperclip',           '~> 2.3.1'
gem 'vpim',                '=  0.695', :require => 'vpim/icalendar'
gem 'action_mailer_tls',   '~> 1.1.3'
gem 'nokogiri',            '~> 1.5.10'
gem 'prawn',               '= 0.11.1'
gem 'memcache-client'
gem "dynamic_form"
gem 'rinku', :require => 'rails_rinku'

group :production do
  gem 'exception_notification'
end

group :development, :test do
  gem 'rspec-rails'
  gem 'factory_girl', '2.6.4'
end

group :development do
  gem 'capistrano',     :require => false
  gem 'capistrano-ext', :require => false

  platform :mri_18 do
    gem 'ruby-debug'
    gem 'ruby18_source_location'
  end

  platform :mri_19 do
    gem 'debugger'
  end

  gem 'pry'
end

group :test do
  gem 'test-unit',        '~> 1.2.3', :require => false
  gem 'cucumber-rails',   :require => false, :git => 'git://github.com/cucumber/cucumber-rails.git', :branch => "rails-2.3.x"
  gem 'database_cleaner', '~> 0.4.3', :require => false
  gem 'webrat',           '~> 0.7.0', :require => false

  platform :mri_18 do
    gem 'rcov', :require => false
  end

  platform :mri_19 do
    gem 'simplecov', :require => false
  end
end
