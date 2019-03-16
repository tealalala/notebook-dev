# Create new Django app

In terminal:

- $1 = project name
  * DO: underscores( _ )
  * DO NOT: hyphens ( - )

## Step 1: Setup and Check Server
```
python3 -m django --version

# create django app
django-admin startproject $1
python3 manage.py startapp $1
python3 manage.py migrate
python3 manage.py runserver
```
## Step 2: Database
If created databases, then do this:

```
python3 manage.py makemigrations
python3 manage.py migrate
```

## Step 3: Database & Python Shell
Test database here:

- $2 = model name (singular)

```
python3 manage.py shell

# output queryset
$2.objects.all()

# create a row in model => autosave
$2.objects.create(title=`title 1`, description=`description 1`)
```
