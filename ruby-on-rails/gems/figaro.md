# Figaro - Ruby Gem
https://github.com/laserlemon/figaro

## Materials
* Rails v5.2.2

## Instructions
In terminal:

- $1 =
- $2 =
- $3 =

### Step 1: Add `figaro` gem and `thor` dependency to Gemfile

```
# project-directory/Gemfile

gem "figaro"
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
