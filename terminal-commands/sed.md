# sed
sed stands for "**s**tream **ed**itor"

```
sed -n '$1,$2p' file-input.txt > file-output.txt  # structure

sed -n '10,20p' file-input.txt > file-output.txt  # example
```

- `-n` - an option that that surpresses printing the input in the terminal
- `$1` - start line
- `$2` - end line
- `file-input.txt` - print from start line and end line from this file
- `>` - redirects file-input.txt prints to file.output.txt
- `file-output.txt` - file-input.txt start line and end line gets printed to file-output.txt