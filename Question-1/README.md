Question 1 – Linux Environment Verification

1. User Identity Verification

Command:
whoami

Output:
siddhu

Explanation:
This command displays the currently logged-in user and confirms my login identity.

Command:
groups

Output:
siddhu adm cdrom sudo dip plugdev users

Explanation:
This command displays all the groups that my user account belongs to, confirming my access permissions.


2. Workspace Validation

Command:
pwd

Output:
/mnt/c/Users/admin

Explanation:
This command displays the current working directory, confirming my present workspace location.

Command:
ls -l

Output:
(Long format listing of files and directories displayed)

Explanation:
This command lists all files and directories in the current location using long format, showing permissions, ownership, size, and timestamps.


3. Environment Confirmation File

Command:
echo "Linux user environment verified" > user_info.txt

Output:
(File created successfully with no terminal output)

Explanation:
This command creates a file named user_info.txt and writes the confirmation message into it to verify the Linux user environment.


4. File Integrity Check

Command:
wc -m user_info.txt

Output:
32 user_info.txt

Explanation:
This command counts the number of characters in user_info.txt, confirming that the file content was written correctly.


5. Learning the Tools

Command:
man mkdir

Useful Option Identified:
-p

Explanation:
The -p option allows creation of parent directories as needed and prevents errors if the directory already exists.


6. Home Directory Inspection

Command:
ls ~

Output:
(No files or directories listed)

Explanation:
This command lists the contents of my home directory. Since it is a new environment, the home directory is empty, so no output was displayed.


7. Log Investigation

Command:
grep "admin" log.txt

Output:
admin logged in

Explanation:
This command searches for the word "admin" inside log.txt and displays only the matching lines.


8. System Information Check

Command:
uname -r

Output:
6.6.87.2-microsoft-standard-WSL2

Explanation:
This command displays the currently running Linux kernel version.


9. Network Connectivity Test

Command:
ping -c 4 www.google.com

Output:
4 packets transmitted, 4 received

Explanation:
This command sends ICMP echo requests to Google to verify network connectivity. The successful replies confirm that the system has internet access.


10. System Health Awareness

Command:
uptime

Output:
(System uptime, number of users, and load average displayed)

Explanation:
The uptime command shows how long the system has been running, the number of logged-in users, and the load average over the last 1, 5, and 15 minutes.
