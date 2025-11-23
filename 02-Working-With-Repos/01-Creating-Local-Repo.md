### 01 - Creating a Local Git Repository

##  What is a Local Repository?
A **local repository** is a Git project stored on your own system.  
It allows you to track changes before pushing anything to GitHub.


##  Step 1: Create a Folder
Create a new project folder anywhere on your computer.

Example:
MyProject


##  Step 2: Open Terminal / Git Bash / VS Code Terminal
Navigate into the folder:

git init

- This creates a hidden `.git` folder inside your project.  
- Now Git starts tracking changes.

Output example:
Initialized empty Git repository in MyProject/.git/


##  Step 4: Create a File
Example:
echo "Hello Git" > file.txt
Or manually create a file in VS Code.


##  Step 5: Check Status
git status

- Shows untracked files  
- Checks what changed


##  Step 6: Stage the File
git add file.txt
(or)
git add .


##  Step 7: Commit the File
git commit -m "First commit"

- Your project is now saved in Git history.


##  Quick Commands Recap
mkdir MyProject
cd MyProject
git init
git status
git add .
git commit -m "First commit"


You created your first local Git repo 
Next: **Connecting Local Repo to GitHub**


