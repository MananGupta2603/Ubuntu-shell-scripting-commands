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
| `hostnamectl`  | Shows or sets the system's hostname          | `hostnamectl`     |
| `uname`        | Prints system information                    | `uname -a`        |
| `arch`         | Displays machine architecture information    | `arch`            |
| `vmstat`       | Reports virtual memory statistics            | `vmstat`          |
| `iostat`       | Reports CPU and I/O statistics               | `iostat`          |
| `mpstat`       | Reports CPU usage per processor              | `mpstat`          |
| `pidstat`      | Reports statistics for Linux tasks           | `pidstat`         |
| `uptime`       | Shows how long the system has been running   | `uptime`          |
| `dmidecode`    | DMI table decoder                            | `sudo dmidecode`  |

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
| `more`         | Views file content one screen at a time           | `more /file`                        |
| `less`         | Views file content with backward movement         | `less /file`                        |
| `head`         | Outputs the first part of files                   | `head -n 10 /file`                  |
| `tail`         | Outputs the last part of files                    | `tail -n 10 /file`                  |
| `chmod`        | Changes file permissions                          | `chmod 755 /file`                   |
| `chown`        | Changes file owner and group                      | `chown user:group /file`            |
| `stat`         | Displays file or file system status               | `stat /file`                        |
| `find`         | Searches for files in a directory hierarchy       | `find /path -name filename`         |
| `locate`       | Finds files by name                               | `locate filename`                   |
| `grep`         | Searches text using patterns                      | `grep 'pattern' /file`              |
| `awk`          | Pattern scanning and processing language          | `awk '/pattern/ {print $0}' /file`  |
| `sed`          | Stream editor for filtering and transforming text | `sed 's/old/new/' /file`            |
| `diff`         | Compares files line by line                       | `diff file1 file2`                  |
| `cmp`          | Compares two files                                | `cmp file1 file2`                   |
| `wc`           | Prints newline, word, and byte counts for files   | `wc /file`                          |

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
| `parted`       | Manipulates disk partitions                       | `sudo parted /dev/sdX`              |
| `lsusb`        | Lists USB devices                                  | `lsusb`                             |
| `lspci`        | Lists PCI devices                                  | `lspci`                             |
| `smartctl`     | Monitors and controls SMART disks                 | `sudo smartctl -a /dev/sdX`         |
| `e2fsck`       | Checks a Linux ext2/ext3/ext4 file system         | `sudo e2fsck /dev/sdX`              |
| `resize2fs`    | Resizes ext2/ext3/ext4 file systems               | `sudo resize2fs /dev/sdX`           |

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
| `id`           | Displays user identity                            | `id username`                       |
| `who`          | Shows who is logged on                            | `who`                               |
| `w`            | Displays who is logged in and what they are doing | `w`                                 |
| `last`         | Shows last logins of users                        | `last`                              |
| `chage`        | Changes user password expiry information          | `sudo chage -l username`            |

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
| `dig`          | DNS lookup utility                                | `dig example.com`                   |
| `hostname`     | Shows or sets the system's hostname               | `hostname`, `hostname newhostname`  |
| `nmcli`        | Command-line client for NetworkManager            | `nmcli dev status`                  |
| `nmtui`        | Text user interface for NetworkManager            | `nmtui`                             |
| `ethtool`      | Displays or changes Ethernet device settings      | `sudo ethtool eth0`                 |
| `iptables`     | Administers IP packet filter rules                | `sudo iptables -L`                  |
| `ss`           | Utility to investigate sockets                    | `ss -tuln`                          |
| `iwconfig`     | Configures wireless network interfaces            | `iwconfig`                          |

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
| `killall`      | Kills all processes by name                       | `killall processname`               |
| `bg`           | Resumes a suspended job in the background         | `bg %1`                             |
| `fg`           | Brings a background job to the foreground         | `fg %1`                             |
| `jobs`         | Lists current jobs                                | `jobs`                              |
| `nice`         | Starts a process with a given priority            | `nice -n 10 command`                |
| `renice`       | Changes the priority of an existing process       | `renice +10 PID`                    |
| `crontab`      | Schedules periodic jobs and tasks                 | `crontab -e`                        |
| `at`           | Schedules a command to run once at a later time   | `at now + 5 minutes`                |
| `batch`        | Executes commands when system load levels permit  | `batch`                             |

## Package Management

| Command        | Description                                       | Example                             |
|----------------|---------------------------------------------------|-------------------------------------|
| `apt-get`      | APT package handling utility                      | `sudo apt-get update`               |
| `apt`          | CLI for the package manager                       | `sudo apt update`, `sudo apt install package` |
| `dpkg`         | Debian package manager                            | `sudo dpkg -i package.deb`          |
| `snap`         | Package management system for snaps               | `sudo snap install package`         |
| `apt-cache`    | Queries APT's package cache                       | `apt-cache search package`          |
| `aptitude`     | Terminal-based UI for APT                         | `sudo apt install aptitude`         |
| `add-apt-repository` | Adds a new repository to APT sources       | `sudo add-apt-repository ppa:repo`  |
| `apt-key`      | Manages APT keys                                  | `sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys key` |
| `snap find`    | Searches for snaps                                | `snap find package`                 |
| `snap list`    | Lists installed snaps                             | `snap list`                         |
| `snap remove`  | Removes a snap package                            | `sudo snap remove package`          |
| `dpkg-reconfigure` | Reconfigures an already installed package    | `sudo dpkg-reconfigure package`     |

## File Compression

| Command        | Description                                       | Example                             |
|----------------|---------------------------------------------------|-------------------------------------|
| `tar`          | Archives files                                    | `tar -cvf archive.tar /path`        |
| `gzip`         | Compresses files                                  | `gzip file`                         |
| `gunzip`       | Decompresses files                                | `gunzip file.gz`                    |
| `zip`          | Package and compress (archive) files              | `zip archive.zip file1 file2`       |
| `unzip`        | Extracts files from a ZIP archive                 | `unzip archive.zip`                 |
| `bzip2`        | Compresses files using Burrows-Wheeler block sorting | `bzip2 file`                      |
| `bunzip2`      | Decompresses bzip2 files                          | `bunzip2 file.bz2`                  |
| `xz`           | Compresses files using the LZMA algorithm         | `xz file`                           |
| `unxz`         | Decompresses xz files                             | `unxz file.xz`                      |
| `7z`           | High compression file archiver                    | `7z a archive.7z file1 file2`       |
| `rar`          | Archive manager for RAR files                     | `rar a archive.rar file1 file2`     |
| `unrar`        | Extracts RAR archive files                        | `unrar x archive.rar`               |

## Conclusion

This cheat sheet covers a wide range of Ubuntu commands that are useful for system administration, file management, network configuration, and more. Use these commands to efficiently manage and troubleshoot your Ubuntu system.
