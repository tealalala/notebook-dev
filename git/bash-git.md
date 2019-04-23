# Bash Functions for Git

## Materials
* Git

## Instructions
In `.bash_profile`:

```
# .bash_profile
gcommit() {
  git add $3
  git status -s
  git commit -m "$4"
  git status -s
  echo "########## COMPLETED ACTIONS: git add and git commit ##########"
}

gpush() {
  git push $1
  git log --oneline -n 5
  echo "########## COMPLETED ACTIONS: git push ##########"
}
```

Call the Bash function:

```
# in the terminal
gcommit --all "this is my commit" # the gcommit function runs and outputs here

gpush origin Master               # or wherever you want to push
```
