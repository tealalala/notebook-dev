# Merge Feature to Master Branch

## Materials
* Git

## Instructions
In terminal:

* $1 = feature branch name

```
# if on $1 first
git pull origin master
git checkout master
git merge $1
git push origin master

git log --oneline -n 5

# delete local branch
git branch -D $1

# delete remote branch
git push origin --delete $1
git push origin :$1
```
