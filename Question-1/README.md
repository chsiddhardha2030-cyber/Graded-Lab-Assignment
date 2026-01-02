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

3. Learning the Tools

Command:
man mkdir

Useful Option Identified:
-p

Explanation:
The -p option allows creation of parent directories as needed and prevents errors if the directory already exists.

4. Home Directory Inspection

Command:
ls ~

Output:
(No files or directories listed)

Explanation:
This command lists the contents of my home directory. Since it is a new environment, the home directory is empty, so no output was displayed.


