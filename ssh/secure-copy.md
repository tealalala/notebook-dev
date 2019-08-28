# Secure Copy (`scp`)
* acronym stands for "Secure Copy"

## Materials
* Terminal

## Instructions
Start in the local folder to copy to remote server

* $1 = local folder absolute path
* $2 = remote server login
* $3 = remote server folder absolute path

```
scp -rp $1 $2:$3
```
* `-r` => recursively (adds all directories)
* `-p` => preserves modification and access times of original file
