Question 3 – Links and Disk Usage

1. File Creation

Command:
echo "This is some sample data for link testing." > sample_data.txt

Output:
(File created successfully with no terminal output)

Explanation:
This command creates a file named sample_data.txt in my home directory and writes sample text into it.


2. Hard Link Creation

Command:
ln sample_data.txt sample_hard.txt

Output:
(Hard link created successfully with no terminal output)

Explanation:
This command creates a hard link named sample_hard.txt that points to the same inode as sample_data.txt.


3. Symbolic Link Creation

Command:
ln -s sample_data.txt sample_soft.txt

Output:
(Symbolic link created successfully with no terminal output)

Explanation:
This command creates a symbolic (soft) link named sample_soft.txt that points to sample_data.txt.


4. Inode Verification

Command:
ls -li sample_data.txt sample_hard.txt sample_soft.txt

Output:
(Inode numbers displayed for all three files)

Explanation:
This command displays the inode numbers along with detailed file information for the original file, hard link, and symbolic link.


5. Inode Analysis

Observation:
sample_data.txt and sample_hard.txt share the same inode number, while sample_soft.txt has a different inode number.

Explanation:
Hard links point to the same inode as the original file, whereas symbolic links are separate files that reference the original file path.


6. File Metadata Inspection

Command:
ls -l sample_data.txt

Output:
(Detailed permissions, ownership, size, and timestamps displayed)

Explanation:
This command displays detailed metadata of sample_data.txt, including permissions, ownership, file size, and timestamps.


7. Disk Usage Check

Command:
du -sh ~

Output:
(Total disk usage of the home directory displayed)

Explanation:
This command shows the total disk space used by the home directory in a human-readable format.


8. File Size Overview

Command:
ls -lh ~

Output:
(List of files in the home directory with human-readable sizes)

Explanation:
This command displays the size of each file in the home directory in a human-readable format.


9. Link Deletion Test

Command:
rm sample_soft.txt

Output:
(Symbolic link deleted successfully)

Explanation:
This command deletes only the symbolic link. The original file sample_data.txt remains unaffected.

Verification Command:
ls sample_data.txt

Explanation:
This confirms that deleting the symbolic link does not affect the original file.


10. Disk Utility Demonstration

Commands:
du -sh ~
du -h --max-depth=1 ~
df -h

Output:
(Disk usage and filesystem information displayed)

Explanation:
The du commands show disk usage of directories and files, while df displays total disk space, used space, available space, and filesystem information in a human-readable format.
