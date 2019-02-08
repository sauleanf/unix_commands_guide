# Unix Command Cheat Sheet

## Key
* [How to manipulate files and directories](#file-and-directory-manipulation)
* [How to edit users](#users)
* [How to update packages and the OS](#update-linux)


## File and Directory Manipulation

Move files

```bash
$ mv filename new_location/filename
```

Rename Files

```bash
$ mv filename new_filename
```

Edit Files

```bash
$ nano filename
```

Create a new file

```bash
$ touch new_filename
or
$ nano new_filename
```

List the content of the current directory

```bash
$ ls
```

Create a new directory

```bash
$ mkdir directory_name
```

Get the current directory

```bash
$ pwd
```

Delete a file or directory

```bash
$ rm -rf filename
or
$ rm -rf directory_name
```

## Users

Create New User

```bash
$ mv sudo adduser username
```

Make an User a SUDOer

```bash
$ sudo usermod -aG sudo username
```

Check the privileges of the current user

```bash
$ sudo -l
```

Check the privileges of the an user

```bash
$ sudo -l -U username
```

Switch users

```bash
$ su - username
```

Change the name of an user

```bash
$ sudo usermod -l new_username username
```

Change the password of an username

```bash
$ passwd username
```

Change your own username

```bash
$ passwd 
```

Delete the username 

```
$ userdel username
```

## Update Linux

Updates the version information of the packages installed on the machine

```bash
$ sudo apt-get update
```
Update the necessary packages by installing new necessary dependencies and removing old unnecessary dependencies. dist-upgrade is essentially a "smart" version of the upgrade tool.

```bash
$ sudo apt-get dist-upgrade
```

Update the all packages but does not install new necessary dependencies nor remove old unnecessary dependencies. 

```bash
$ sudo apt-get upgrade
```

BOTH DIST-UPGRADE AND UPGRADE NEED TO RAN AFTER UPDATE.

How to upgrade to the recent version of the Linux Distribution (Ubuntu only)

```bash
$ sudo do-release-update
```

## Networking

How to get your local ip

```bash
$ ip route get 8.8.8.8 | awk '{print $NF; exit}'
```
