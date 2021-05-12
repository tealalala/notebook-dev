# Basic Handling: Branch, Rebase and Merge Request to Master

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

# delete feature-branch
git branch -D feature-branch            # delete local branch
git push origin --delete feature-branch # delete remote branch
git fetch --all --prune                 # clean up branches and local branches

# if on feature-branch first
git pull origin master
git checkout master
git merge feature-branch
git push origin master
git log --oneline -n5

# git pull
git pull                # runs git fetch + git merge
git pull --rebase       # runs git fetch + git rebase

# rebase master into feature branch
git fetch                 # receive latest changes from remote git repo
git rebase origin/master  # integrate changes from master into feature
git add .                 # stage changes
# NOTE: do not run git commit, since we're just integrating master to feature, not committing anything new
git rebase --continue     # after resolving conflicts (if any), continue with rebase
git rebase --abort        # cancel rebasing rather than resolve conflicts
git push                  # push rebased changes into feature, 
                          # may need to do `git push --force` (do this if you're the only one working on your feature branch)

# create merge request
git checkout master
git pull
git merge feature-branch
git push origin master
```