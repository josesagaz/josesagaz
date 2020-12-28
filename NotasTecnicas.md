# Technical Notes

## 🔥 SSH Login Without Password 
Generate a key pair on the local server
```
ssh-keygen
```

Install your public key on the remote server
```
ssh-copy-id -i ~/.ssh/id_rsa.pub UserName@RemoteServer
```

Add a private key to the authentication agent on the local server
```
ssh-add
```

## 🔥 Add User to Sudoers in Debian
```
usermod -aG sudo username
```
