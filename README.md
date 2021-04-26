# Hotwire Chat Demo

Following [demo](https://hotwire.dev) from Hotwire home page.

## Original project setup
- `lando start`
- `lando rails new . --skip-javascript`
- Add `gem 'hotwire-rails'` to Gemfile and run `lando bundle`
- `lando rails hotwire:install`
- `lando bundle` again to install redis specified from hotwire
- `lando rails g scaffold room name:string`
- `lando rails g model message room:references content:text`
- `lando rails db:migrate RAILS_ENV=development`
- Follow video to add messages templates and partial, add to room files.
- Add `config.hosts << "hotwire-chat.lndo.site"` to config/environments/development.rb
