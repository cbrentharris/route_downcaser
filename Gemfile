source "http://rubygems.org"

gemspec

###############################################
# Enable testing of multiple rails versions
rails_version = ENV["RAILS_VERSION"] || "default"
rails = case rails_version
when "master"
  {github: "rails/rails"}
when "default"
  ">= 3.1.0"
else
  "~> #{rails_version}"
end
gem "rails", rails
###############################################

###############################################
# The following gems are also needed to test within the Rails env
gem 'jquery-rails'
gem 'turbolinks'
###############################################

gem "codeclimate-test-reporter", group: :test, require: nil
