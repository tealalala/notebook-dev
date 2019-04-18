# Figaro - Ruby Gem
gem figaro: https://github.com/laserlemon/figaro
https://richonrails.com/articles/configuration-management-with-figaro
gem pusher: https://github.com/pusher/pusher-http-ruby

## Materials
* Rails v5.2.2

## Instructions
In terminal:

### Step 1: Add `figaro` gem and `thor` dependency to Gemfile

```
# project-directory/Gemfile

gem 'figaro'
gem 'thor', '~> 0.20.3'
```

### Step 2: Install `figaro` + dependencies

```
bundle install
bundle exec figaro install   # create config/application.yml and adds to .gitignore
```

* After running the above, run a rails command to test if works: `rails c`

### Step 3: Edit config/application.yml
* edit with own keys and secrets

```
# config/application.yml

pusher_app_id: "2954"
pusher_key: "7381a978f7dd7f9a1117"
pusher_secret: "abdc3b896a0ffb85d373"
```
* After running the above, run a rails command to test if works: `rails c`

### Step 4: Use `Figaro.env` over regular `ENV` due to stubbing and unstubbing during testing
* then when `application.yml` is accessed, Figaro loads the setting from `application.yml`

```
# config/secrets.yml

Figaro.env.stripe_api_key # => "sk_live_dSqzdUq80sw9GWmuoI0qJ9rL"
Figaro.env.stripe_api_key? # => true
Figaro.env.google_analytics_key # => nil
Figaro.env.google_analytics_key? # => false
```
* test this in `rails console`:

```
Rails.application.secrets.secret_key_base
Figaro.env.secret_key_base
ENV['secret_key_base']
```

### Step 5: Add gem `pusher` to push environmental variables from ENV => Figaro => initializers to verify config keys

```
# Gemfile
gem 'pusher', '~> 1.3'

# pusher gem runtime dependencies below
gem 'httpclient', '~> 2.8', '>= 2.8.3'
gem 'multi_json', '~> 1.13', '>= 1.13.1'
gem 'pusher-signature', '~> 0.1.8'

# pusher gem development dependencies
gem 'em-http-request', '~> 1.1', '>= 1.1.5'
gem 'json', '~> 2.2'
gem 'rack', '~> 2.0', '>= 2.0.7'
gem 'rake', '~> 12.3', '>= 12.3.2'
gem 'rspec', '~> 3.8'
gem 'webmock', '~> 3.5', '>= 3.5.1'
```


### Step 6: `require 'pusher'` in `config/initializer/pusher.rb`

```
pusher_client = Pusher::Client.new(
  github_oauth2_client_id: Figaro.env.github_oauth2_client_id!,
  github_oauth2_client_secret: Figaro.env.github_oauth2_client_secret!
)
```

* test command `rails console` or other command to see if Rails app still works
