# Git rebase master to feature

```
git fetch                 # receive latest changes from remote git repo
git rebase origin/master  # integrate changes from master into feature
git add .                 # stage changes
# NOTE: do not run git commit, since we're just integrating master to feature, not committing anything new
git rebase --continue     # after resolving conflicts (if any), continue with rebase
git rebase --abort        # cancel rebasing rather than resolve conflicts
git push                  # push rebased changes into feature
```