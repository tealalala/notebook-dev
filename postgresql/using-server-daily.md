# Daily: Using Postgresql Database Server

## Materials
* Postgresql v11.2

## Instructions
In terminal:

### Step 1: Check Postgresql version
```
brew install postgresql                     # install Postgresql
brew info postgresql                        # learn more about your new package and where it is in the Cellar
psql --version                              # you can also do this to check the version you have
which psql                                  # and do this to check where the file is- turns out the location is different from the cellar's postgresql. hmmm... wonder why?
initdb /usr/local/var/postgres              # create database in your local folder
```

### Step 2 - Manage Database Server
#### Option 1: Manually Start, End and Check Status of Postgres Server
```
pg_ctl -D /usr/local/var/postgres start     # start postgres server
pg_ctl -D /usr/local/var/postgres stop      # stop postgres server
pg_ctl -D /usr/local/var/postgres status    # check the status of the server when you need to
```

#### Option 2: Automatically Start, End and Restart Postgres Server in Brew
```
brew services start postgresql              # start postgres server whenever you logged in
brew services stop postgresql               # stop postgresql server
brew services restart postgresql            # restart the server, if you need to
```
