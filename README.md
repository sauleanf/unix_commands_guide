## File Manipulation

Move files

```bash
$ mv filename new_location/filename
```

Rename Files

```bash
$ mv filename new_filename
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

BOTH DIST-UPGRADE AND UPGRADE NEED TO RAN FROM UPDATE.
