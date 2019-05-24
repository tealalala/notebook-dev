# Basic Handling: Branch and Merge Request to Master

## Materials
* Git

## Instructions
In terminal:

```
# make edits to Branch
git checkout -b my-branch-name

# sub-branch (sub-branch1) of a branch (branch1)
git checkout branch1
git checkout -b sub-branch1 branch1
git push origin sub-branch1

# create merge request
git checkout master
git pull
git merge my-branch-name
git push origin master

# delete my-branch-name
git branch -D my-branch-name            # delete local repo
git push origin --delete my-branch-name # delete remote repo
git fetch --all --prune                 # clean up branches and local repos
```
