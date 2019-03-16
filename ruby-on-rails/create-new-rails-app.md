# Create new Rails app

In terminal:

- $1 = project name
- $2 = controller name (plural)
- $3 = model name (singular)


```
rails new $1
cd $1

# controllers are plural name
rails generate controller api/$2

# models are singular name; key:type - list the table attribute and data type
rails generate model $3 key:type key:type

# create db for $3
rails db:create

bundle install
```
