# Create new Rails app

## Materials
* Rails v5.2.2

## Instructions
In terminal:

- $1 = project name
- $2 = controller name (plural)
- $3 = model name (singular)

```
rails new $1
cd $1

# controllers are plural name
rails generate controller api/$2  # generate controller longform
rails g controller api/$2         # generate controller shortform

# models are singular name; key:type - list the table attribute and data type
rails generate model $3 key:type key:type

# create db for $3
rails db:create

bundle install
```
