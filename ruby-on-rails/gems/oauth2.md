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

gem "oauth2"
gem "faraday", "~> 0.15.4"
gem "multipart-post", "~> 2.0"
gem "multi_json", "~> 1.13", ">= 1.13.1"
gem "multi_xml", "~> 0.6.0"
gem "rack", "~> 2.0", ">= 2.0.7"
```

### Step 2: Install `oauth2` and other runtime dependencies

```
bundle install
```
