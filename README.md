
# Ubuntu Commands Cheat Sheet

This cheat sheet provides a comprehensive list of Ubuntu commands, categorized by their functions. It includes commands for system information, file management, disk management, user management, network management, process management, package management, and file compression.

## Table of Contents

1. [System Information](#system-information)
2. [File Management](#file-management)
3. [Disk Management](#disk-management)
4. [User Management](#user-management)
5. [Network Management](#network-management)
6. [Process Management](#process-management)
7. [Package Management](#package-management)
8. [File Compression](#file-compression)

## System Information

| Command        | Description                                  | Example           |
|----------------|----------------------------------------------|-------------------|
| `uname`        | Prints detailed system information           | `uname -a`        |
| `df`           | Reports disk space usage of the file system  | `df -h`           |
| `du`           | Checks disk usage of files and directories   | `du /path`        |
| `top`          | Displays a dynamic view of system processes  | `top`             |
| `htop`         | Interactive process viewer                   | `htop`            |
| `free`         | Displays memory usage                        | `free -h`         |
| `uptime`       | Shows how long the system has been running   | `uptime`          |
| `dmesg`        | Prints kernel ring buffer messages           | `dmesg`           |
| `lshw`         | Lists hardware configuration                 | `lshw`            |
| `lsblk`        | Lists information about block devices        | `lsblk`           |
| `inxi`         | Displays comprehensive system information    | `inxi`            |

## File Management

| Command        | Description                                       | Example                             |
|----------------|---------------------------------------------------|-------------------------------------|
| `ls`           | Lists directory contents                          | `ls -l`, `ls -a`                    |
| `cp`           | Copies files or directories                       | `cp /source /destination`           |
| `mv`           | Moves or renames files or directories             | `mv /source /destination`           |
| `rm`           | Removes files or directories                      | `rm /file`, `rm -r /directory`      |
| `mkdir`        | Creates a new directory                           | `mkdir /directory`                  |
| `rmdir`        | Removes empty directories                         | `rmdir /directory`                  |
| `touch`        | Creates an empty file or updates the timestamp    | `touch /file`                       |
| `ln`           | Creates hard or symbolic links                    | `ln /source /link`, `ln -s /source /link` |
| `cat`          | Concatenates and displays file content            | `cat /file`                         |
| `nano`         | Opens the nano text editor                        | `nano /file`                        |

## Disk Management

| Command        | Description                                       | Example                             |
|----------------|---------------------------------------------------|-------------------------------------|
| `fdisk`        | Partition table manipulator for Linux             | `sudo fdisk -l`                     |
| `mkfs`         | Builds a Linux file system                        | `mkfs.ext4 /dev/sdX`                |
| `mount`        | Mounts a file system                              | `sudo mount /dev/sdX /mnt`          |
| `umount`       | Unmounts a file system                            | `sudo umount /mnt`                  |
| `lsblk`        | Lists information about block devices             | `lsblk`                             |
| `blkid`        | Lists UUIDs of block devices                      | `blkid`                             |
| `df`           | Reports file system disk space usage              | `df -h`                             |
| `du`           | Estimates file and directory space usage          | `du -sh /path`                      |

## User Management

| Command        | Description                                       | Example                             |
|----------------|---------------------------------------------------|-------------------------------------|
| `adduser`      | Adds a user to the system                         | `sudo adduser username`             |
| `useradd`      | Adds a user to the system (lower-level command)   | `sudo useradd username`             |
| `usermod`      | Modifies a user account                           | `sudo usermod -aG group username`   |
| `passwd`       | Updates a user's password                         | `sudo passwd username`              |
| `deluser`      | Removes a user from the system                    | `sudo deluser username`             |
| `groupadd`     | Adds a new group                                  | `sudo groupadd groupname`           |
| `groupdel`     | Deletes a group                                   | `sudo groupdel groupname`           |

## Network Management

| Command        | Description                                       | Example                             |
|----------------|---------------------------------------------------|-------------------------------------|
| `ifconfig`     | Configures network interfaces (deprecated)        | `ifconfig`                          |
| `ip`           | Shows/manipulates routing, devices, and tunnels   | `ip a`, `ip r`                      |
| `ping`         | Sends ICMP ECHO_REQUEST to network hosts          | `ping example.com`                  |
| `traceroute`   | Prints the route packets take to the network host | `traceroute example.com`            |
| `netstat`      | Network statistics                                | `netstat -tuln`                     |
| `nslookup`     | Queries internet name servers interactively       | `nslookup example.com`              |
| `wget`         | Non-interactive network downloader                | `wget http://example.com/file.zip`  |
| `curl`         | Transfers data from or to a server                | `curl http://example.com`           |
| `scp`          | Secure copy (remote file copy program)            | `scp file user@remote:/path`        |
| `ssh`          | OpenSSH remote login client                       | `ssh user@remote`                   |

## Process Management

| Command        | Description                                       | Example                             |
|----------------|---------------------------------------------------|-------------------------------------|
| `ps`           | Reports a snapshot of current processes           | `ps aux`                            |
| `pstree`       | Displays a tree of processes                      | `pstree`                            |
| `kill`         | Sends a signal to a process                       | `kill -9 PID`                       |
| `pkill`        | Kills processes by name                           | `pkill processname`                 |
| `top`          | Displays tasks                                    | `top`                               |
| `htop`         | Interactive process viewer                        | `htop`                              |
| `systemctl`    | Manages systemd services                          | `sudo systemctl restart service`    |
| `service`      | Runs a System V init script                       | `sudo service apache2 restart`      |

## Package Management

| Command        | Description                                       | Example                             |
|----------------|---------------------------------------------------|-------------------------------------|
| `apt-get`      | APT package handling utility                      | `sudo apt-get update`               |
| `apt`          | CLI for the package manager                       | `sudo apt update`, `sudo apt install package` |
| `dpkg`         | Debian package manager                            | `sudo dpkg -i package.deb`          |
| `snap`         | Package management system for snaps               | `sudo snap install package`         |
| `apt-cache`    | Queries APT's package cache                       | `apt-cache search package`          |
| `aptitude`     | Terminal-based UI for APT                         | `sudo apt install aptitude`         |

## File Compression

| Command        | Description                                       | Example                             |
|----------------|---------------------------------------------------|-------------------------------------|
| `tar`          | Archives files                                    | `tar -cvf archive.tar /path`        |
| `gzip`         | Compresses files                                  | `gzip file`                         |
| `gunzip`       | Decompresses files                                | `gunzip file.gz`                    |
| `zip`          | Package and compress (archive) files              | `zip archive.zip file1 file2`       |
| `unzip`        | Extracts files from a ZIP archive                 | `unzip archive.zip`                 |

## Conclusion

This cheat sheet covers a wide range of Ubuntu commands that are useful for system administration, file management, network configuration, and more. Use these commands to efficiently manage and troubleshoot your Ubuntu system.
