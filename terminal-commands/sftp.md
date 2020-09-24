# sftp
sftp stands for "secure file transfer program"

$1 = FTP log in username

```
sftp $1              // follow the prompt
sftp>                // you're logged in!
sftp> ls             // try a common command like ls; run commands below to upload/download
sftp>                // exit by pressing on your keyboard: CTRL + D
```

after logging in, you can do any the following commands:

- `get /remote/absolute/directory/* /local/absolute/directory/*` - this downloads files from remote server ==> local machine
- `put /absolute/directory/*` - this uploads the files from your local machine ==> remote server