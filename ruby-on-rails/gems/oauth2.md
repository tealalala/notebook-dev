# OAuth2 - Ruby Gem
Last Updated: 04/09/2019

* Official: https://github.com/oauth-xx/oauth2
* Gem: https://rubygems.org/gems/oauth2/

## Materials
* Rails v5.2.2

## Instructions

### Step 1: Add `oauth2` gem and other runtime dependencies to Gemfile
* NOTE: development dependencies NOT included below

```
# project-directory/Gemfile

gem 'oauth2'

# runtime dependencies
gem 'faraday', '~> 0.15.4'
gem 'multipart-post', '~> 2.0'
gem 'multi_json', '~> 1.13', '>= 1.13.1'
gem 'multi_xml', '~> 0.6.0'
gem 'rack', '~> 2.0', '>= 2.0.7'

# dev dependencies
gem 'addressable', '~> 2.6'
gem 'backports', '~> 3.13'
gem 'coveralls', '~> 0.8.22'
gem 'rdoc', '~> 6.1', '>= 6.1.1'
gem 'rspec', '~> 3.8'
gem 'wwtd', '~> 1.3'

```

### Step 2: Install `oauth2` and other runtime dependencies

```
bundle install
```

### Step 3: Determine Parameters

* `client_id`
* `redirect_uri`
* `login`
* `scope`
* `state`
* `allow_signup`
