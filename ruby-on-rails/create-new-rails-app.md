# Create new Rails app

In terminal:

$1 = project name
$2 = controller name (plural)
$3 = model name (singular)


```
rails new $1
cd $1
rails generate controller api/$2	          # controllers are plural name
rails generate model $3 key:type key:type   # models are singular name; key:type - list the table attribute and data type
rails db:create			                        # create db for $3
bundle install
```
