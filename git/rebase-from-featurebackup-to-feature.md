# Git rebase from feature backup to feature

```
git checkout -b feature-backup
git fetch origin              # updates tracking branches
git rebase origin/feature     # rebase from feature backup to feature
```