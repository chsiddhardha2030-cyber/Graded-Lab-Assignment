Question 2 – File and Directory Management

1. Project Workspace Setup

Command:
mkdir ~/documents

Output:
(Directory created successfully with no terminal output)

Explanation:
This command creates a directory named documents inside my home directory to store project-related files.


2. File Creation

Command:
cd ~/documents
touch plan.txt

Output:
(File plan.txt created successfully with no terminal output)

Explanation:
The cd command navigates into the documents directory, and the touch command creates an empty file named plan.txt.


3. Content Addition

Command:
echo "This is the initial project plan." > plan.txt

Output:
(Text written to file with no terminal output)

Explanation:
This command writes sample project-related text into the plan.txt file.


4. File Metadata Verification

Command:
ls -l plan.txt

Output:
-rw-r--r-- 1 siddhu siddhu ... plan.txt

Explanation:
This command displays file permissions, ownership, and metadata. The output confirms that the file is owned by my user account.


5. File Duplication

Command:
cp plan.txt plan_copy.txt

Output:
(File copied successfully with no terminal output)

Explanation:
This command creates a duplicate of plan.txt named plan_copy.txt.


6. Directory Renaming

Command:
cd ~
mv documents project_documents

Output:
(Directory renamed successfully with no terminal output)

Explanation:
This command renames the documents directory to project_documents to better reflect the project scope.


7. Archival Structure

Command:
mkdir ~/project_documents/archive

Output:
(Archive directory created successfully with no terminal output)

Explanation:
This command creates a subdirectory named archive inside project_documents to store archived files.


8. File Organization

Command:
mv ~/project_documents/plan_copy.txt ~/project_documents/archive/

Output:
(File moved successfully with no terminal output)

Explanation:
This command moves plan_copy.txt into the archive subdirectory for proper organization.


9. Recursive Listing

Command:
ls -R ~/project_documents

Output:
(Complete directory structure displayed recursively)

Explanation:
This command lists all files and subdirectories inside project_documents recursively, showing the entire directory hierarchy.


10. Path Verification

Command:
realpath ~/project_documents/archive/plan_copy.txt

Output:
/home/siddhu/project_documents/archive/plan_copy.txt

Explanation:
This command displays the absolute path of plan_copy.txt after it has been moved to the archive directory.
