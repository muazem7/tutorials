# Bash Commands
## 1. File & Directory Management
- `ls` **- List directory contents**
- `cd [dir]` **- Change directory** 
- `pwd` **- Print current directory**  
- `mkdir [dir]` **- Create a new directory**  
- `rm [file]` **- Remove a file**  
- `rm -r [dir]` **- Remove a directory recursively**  
- `cp [src] [dest]` **- Copy files or directories**  
- `mv [src] [dest]` **- Move or rename files/directories**  
- `touch [file]` **- Create an empty file**  
- `find [dir] -name [filename]` **- Search for a file**  

## 2. File Viewing & Editing
- `cat [file]` **- View file content**  
- `file [file]` **- Determine file type**  
- `less [file]` **- View file content (scrollable)**  
- `head -n [num] [file]` **- View first N lines**  
- `tail -n [num] [file]` **- View last N lines**  
- `nano [file]` **- Edit file using nano**  
- `vim [file]` **- Edit file using Vim**  

## 3. File Permissions & Ownership
- `ls -l` **- View file permissions**  
- `chmod 755 [file]` **- Change file permissions**  
- `chown user:group [file]` **- Change file owner**  

## 4. Process Management
- `ps aux` **- View running processes**  
- `top` **- Display active processes**  
- `htop` **- Interactive process manager**  
- `kill [PID]` **- Kill a process**  
- `killall [process_name]` **- Kill all processes by name**  
- `pkill [name]` **- Kill process by name**  

## 5. Disk Management
- `df -h` **- Show disk usage**  
- `du -sh [dir]` **- Show directory size**  
- `lsblk` **- Display information about block devices**  

## 6. Search & Text Processing
- `grep [pattern] [file]` **- Search for a pattern in a file**  
- `sort [file]` **- Sort lines in a file**  
- `uniq [file]` **- Remove duplicate lines**  
- `strings [file]` **- Extract readable text from binary files**  
- `base64 [file]` **- Encode/decode files in Base64**  
- `tr [set1] [set2]` **- Translate or delete characters**  
- `jq [filter] [file]` **- Process and format JSON data**
  
## 7. Archiving & Compression
- `tar -cvf archive.tar [dir]` **- Create a tar archive**  
- `tar -xvf archive.tar` **- Extract a tar archive**  
- `gzip [file]` **- Compress a file**  
- `bzip2 [file]` **- Compress a file using bzip2**  
- `xxd [file]` **- Create a hex dump of a file**  

## 8. User Management
- `whoami` **- Show current user**  
- `who` **- Show logged-in users**  
- `sudo [command]` **- Run command as superuser**  
- `su [user]` **- Switch user**  
- `useradd [user]` **- Add a new user**  
- `passwd [user]` **- Change user password**  
- `groupadd [group]` **- Create a group**  
- `usermod -aG [group] [user]` **- Add user to group**  

## 9. System Monitoring & Logs
- `uptime` **- Show system uptime**  
- `free -m` **- Show memory usage**  
- `df -h` **- Show disk space usage**  
- `dmesg` **- Show system logs**  
- `journalctl -xe` **- View detailed logs**  

## 10. Scripting & Automation
- `chmod +x script.sh` **- Make script executable**  
- `cron` **- Schedule jobs at fixed times**  
- `crontab -e` **- Edit cron jobs**  
