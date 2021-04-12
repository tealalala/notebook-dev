# Git pull from master to feature

```
git checkout feature-branch
git fetch origin                  # fetch the origin, and review the commits
git merge origin/master --no-ff   # merge to feature branch, --no-ff can be --ff
```