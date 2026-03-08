# Linux for Cybersecurity

This repository contains Linux commands and concepts useful for cybersecurity, penetration testing, and system investigation.

Linux is widely used in cybersecurity tools, servers, and penetration testing environments such as Kali Linux.

## Topics Covered

- File navigation
- File permissions
- Process monitoring
- Networking commands
- Log analysis

These commands are commonly used during system enumeration, incident response, and penetration testing.

## File Navigation

pwd  
Displays the current working directory.

ls  
Lists files and directories.

ls -la  
Lists all files including hidden files with detailed permissions.

cd /directory  
Changes the current working directory.

## File Searching

find  
Searches for files and directories within a directory hierarchy.

Example:
find /home -name file.txt

Search for files with a specific extension:
find / -name "*.conf"

## File Permissions

chmod  
Changes file permissions.

Example:
chmod +x script.sh

Makes a file executable.

chown  
Changes file ownership.

Example:
chown user:file filename

## Text Searching

grep  
Searches for specific text patterns inside files.

Example:
grep "error" logfile.txt

Search recursively inside directories:
grep -r "password" /etc

Example for log investigation:
grep "failed password" /var/log/auth.log

## File Viewing

cat  
Displays the contents of a file.
tail  
Displays the last lines of a file.
head  
Displays the first lines of a file.
less  
Displays file content one page at a time.

## Text Processing

awk  
Used for pattern scanning and text processing.

Example:
awk '{print $1}' file.txt
sed  
Stream editor used to modify text.

Example:
sed 's/error/warning/g' file.txt

## Process Monitoring

ps aux  
Displays all running processes.

top  
Shows real-time process activity.

kill PID  
Terminates a running process.

## Networking Commands

ifconfig  
Displays network interface information.

ip a  
Shows IP addresses and network interfaces.

netstat -tulnp  
Displays listening ports and network services.

## Log Analysis

cat /var/log/auth.log  
Displays authentication logs.

grep "failed" /var/log/auth.log  
Searches logs for failed login attempts.

tail -f /var/log/syslog  
Monitors logs in real time.


