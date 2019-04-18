# Basic Handling: Install & Deploy

## Materials
* brew
  * Heroku - installed by brew
  * Git - works in tandem with Heroku

## Instructions
In terminal:

- $1 = github address to project
- $2 = git commit message
- $3 = rails master key

```
# install
brew install heroku/brew/heroku

# setup - login with heroku
heroku login

# git commit and push, then deploy rails app to heroku
git add --all
git commit -m "$2"
git push origin master

heroku create
git push heroku master
eroku run rails db:migrate
heroku run rails db:seed
heroku config:set RAILS_MASTER_KEY=$3
heroku open


# git commit and push, then update rails app to heroku
heroku
git add --all
git commit -m "$2"
git push origin master
git push heroku master
```
