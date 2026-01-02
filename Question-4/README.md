Question 4 – System Monitoring and Process Management

1. System Uptime Verification

Command:
uptime

Output:
(System uptime displayed)

Explanation:
This command displays the time elapsed since the system was last booted.


2. User Process Listing

Command:
ps -u $USER

Output:
(List of processes running under the current user)

Explanation:
This command lists all processes currently running under my user account.


3. CPU Usage Analysis

Command:
top -u $USER

Output:
(Process list with CPU usage displayed)

Explanation:
This command displays running processes for my user and allows identification of the process consuming the highest CPU.


4. Background Process Execution

Command:
sleep 300 &

Output:
(Background job started with job number and PID)

Explanation:
This command starts a process in the background and confirms that it is running.


5. Process Priority Management

Commands:
ps -u $USER | grep sleep
renice 10 -p 4529
ps -o pid,ni,cmd -p 4529

Output:
(Process priority changed from 0 to 10)

Explanation:
These commands identify a running process, change its niceness value, and verify the updated priority.


6. Memory Usage Monitoring

Command:
free -h

Output:
(Memory usage displayed in human-readable format)

Explanation:
This command displays total, used, and free system memory in a human-readable format.


7. Disk Space Inspection

Command:
df -h ~

Output:
(Disk space usage of the filesystem containing the home directory)

Explanation:
This command shows disk space usage of the filesystem where my home directory resides.


8. Shell Identification

Command:
echo $SHELL

Output:
/bin/bash

Explanation:
This command displays the name of the shell currently in use.


9. Output Redirection

Commands:
uname -a > system_report.txt
cat system_report.txt

Output:
(System information written to and displayed from system_report.txt)

Explanation:
These commands redirect system information into a file and verify its contents.


10. Disk Usage Visualization (ncdu)

Command:
ncdu ~

Output:
(ncdu command not found on this system)

Explanation:
The ncdu utility is not installed on this system and installing new software is not permitted. Normally, ncdu provides an interactive disk usage visualization showing which directories and files consume the most space. It is commonly used with commands like 'ncdu ~' to analyze disk usage interactively.
