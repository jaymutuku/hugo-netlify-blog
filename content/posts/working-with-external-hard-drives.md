---
title: Fixing NTFS hard drive that refuses to mount
date: 2020-11-08
tags: [troubleshooting]
description: how to fix NTFS hard drive that refuses to mount
draft: false
---

### Fixing NTFS hard drive that refuses to mount 
This could be that is is not automounting coz of an error to do
with bad sectors etc.

```
$ yes | sudo pacman -S ntfs-3g

```
Then

```
$ sudo ntfsfix /dev/sdX
```
where `/dev/sdX` is the Hard Drive e.g `/dev/sdd1`

###  Checking the type of your mounted partitions or devices

```
$ sudo blkid /dev/sdd
```
Where `/dev/sdd1` is your

### Check your mounted partitions/devices
```
$ cat /proc/mounts
```

```
$ cat /etc/fstab
```
### mount device(hard drive) using terminal
```
$ sudo mount -t ntfs /dev/sdd1 /mnt
```
### unmount device from  using terminal 

```
$ sudo umount /dev/sdd1
```