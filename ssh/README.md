## copy files from remote server to local (two layers of host)
### 1. create a file ~/.ssh/config which contains: \

```
Host ae
HostName ssh.ae.gatech.edu
PreferredAuthentications publickey
# IdentityFile id_rsa
User hyu419

Host hz
Hostname ae-scml-406200
ProxyJump ae
User hyu419
```

### 2. copy
scp user@hz:path_to_file local_path_to_file

