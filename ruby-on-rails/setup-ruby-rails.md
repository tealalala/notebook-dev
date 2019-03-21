# Setup Environment with Homebrew-rbenv and rbenv-(Ruby and Ruby on Rails)

## Materials
First, we'll install:

| Item     | Version | Location             | Note             |
| -------- | ------- | -------------------- | ---------------- |
| Homebrew | 2.0.5   | /usr/local/bin/brew  | package mgr      |

Second, we'll install `rbenv` with `brew`:

| Item     | Version | Location             | Note             |
| -------- | ------- | -------------------- | ---------------- |
| rbenv    | 1.1.1   | /usr/local/bin/rbenv | ruby version mgr |

Third, we'll install with `rbenv`:
* $1 = computer name

| Item           | Version | Location                                   |
| -------------- | ------- | -------------------------------------------|
| Bundle         | 2.5.1   | /Users/$1/.rbenv/versions/2.5.1/bin/bundle |
| gem (rubygems) | 3.0.3   | /Users/$1/.rbenv/versions/2.5.1/bin/gem    |
| Rails          | 5.2.2.1 | /Users/$1/.rbenv/shims/rails               |
| Ruby           | 2.5.1   | /Users/$1/.rbenv/shims/ruby                |

## Instructions
### Step 1: Install `brew`

```
# Install Homebrew
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

# Install rbenv
brew install rbenv
```

### Step 2: Install `rbenv` with `brew`
`rbenv` creates **shims** for all Rails commands (`ruby`, `irb`, etc.) across all versions of Ruby. This process is called rehashiing. Make sure to run `rbenv rehash` when new commands are shimmed.
```
# Install Homebrew
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

# Install rbenv
brew install rbenv
```

### Step 3: Install `rubygems`, `rails`, `ruby` with `rbenv`
* See above for installation locations.

```
# rubygems should already be installed with ruby via ruby-build from Homebrew

gem update --system   # update rubygems only, if needed
rbenv install 2.5.1   # installs specific version of ruby
rbenv install rails   # install rails, recent version
```

### Step 4: Switch Ruby version in different environments
DO THIS:
  * `rbenv shell` => set ruby version temporarily in the shell
  * `rbenv local` => set ruby version in project
  * `rbenv global` => set ruby version on global

```
# using `rbenv shell`
ruby -v
rbenv shell 2.5.1
ruby -v

# using `rbenv local`
ruby -v
rbenv local 2.5.1
ruby -v

# using `rbenv global`
ruby -v
rbenv global 2.5.1
ruby -v

```
