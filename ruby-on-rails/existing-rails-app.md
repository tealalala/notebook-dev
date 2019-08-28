# Working on an Existing Rails App

## Materials
* Rails v5.2.2

## Instructions

### In terminal:

- $1 = project github
- $2 = ruby version for Rails app

```
git clone $1
rails db:create
rails db:migrate

rbenv local $2
bundle install

brew services start postgresql
```

### In Postico:
Add below and everything else can be empty:

```
Database: postgres
```

Click **connect** to start the PostgreSQL server with Postico.
