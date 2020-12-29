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

## 🔥 Mount usb drive
```
sudo fdisk -l
```
Should show the USB drive like
```Device Boot Start End Blocks Id System
/dev/sdb1 * 32 30595071 15297520 c W95 FAT32 (LBA)```


```
sudo mount /dev/sdb1 /mnt
```

Format USB with vFat File System
```
$ sudo mkfs.vfat /dev/sdb1
```

Format NTFS FileSystem
```
$ sudo mkfs.ntfs /dev/sdb1
```

Format EXT4 FileSystem
```
$ sudo mkfs.ext4 /dev/sdb1
```
