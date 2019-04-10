# .bashrc
* Path: /Users/usernamehere
* $1 = indicates username

```
# Mosh
alias mosh="mosh --server=\"LD_LIBRARY_PATH=/home/$1/lib /home/$1/bin/mosh-server\""

# ?
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"  # This loads nvm
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"  # This loads nvm bash_completion

# Homebrew
if type brew 2&>/dev/null; then
  for completion_file in $(brew --prefix)/etc/bash_completion.d/*; do
    source "$completion_file"
  done
fi
```
