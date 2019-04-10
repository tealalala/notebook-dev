# .gitconfig
* Path: /Users/usernamehere
* $1 = github username
* $2 - github email

```
[user]
  name = $1
  email = $2
[filter "lfs"]
  clean = git-lfs clean -- %f
  smudge = git-lfs smudge -- %f
  process = git-lfs filter-process
  required = true
[color]
  ui = true
[credential]
  helper = osxkeychain
```
