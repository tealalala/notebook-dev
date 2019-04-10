# .bash_profile
* Path: /Users/usernamehere

```
# Brew PATH
export PATH="/usr/local/sbin:$PATH"

# Python 3.7 PATH
# The original version is saved in .bash_profile.pysave
PATH="/Library/Frameworks/Python.framework/Versions/3.7/bin:${PATH}"
export PATH

# Ruby version
export PATH="/usr/local/opt/ruby/bin:$PATH"

# Rbenv - Ruby Language
if which rbenv > /dev/null; then eval "$(rbenv init -)"; fi
eval "$(rbenv init -)"

# Terminal colors
export CLICOLOR=1
export LSCOLORS=GxFxCxDxBxegedabagaced
export PS1="\[\033[36m\]\w\[\033[0m\]$ "
export EDITOR='subl -w'
alias ls='ls -GFh'

# display current directory folder only, not path relative to user root
PS1='\[\033[01;34m\][\W]\[\033[00m\]$ '
```
