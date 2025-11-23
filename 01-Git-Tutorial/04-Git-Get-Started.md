### 04 – Git Get Started

# 1. What Does “Getting Started” Mean?

This is all about:
- Checking if Git is installed
- Creating your first folder/project
- Turning that folder into a Git repository
- Understanding basic Git workflow

This is your FIRST real Git hands-on step.


# 2. Check if Git is Installed

Open Git Bash / Terminal and run:

git --version

# If Git is installed, you will see something like:

git version 2.45.0

# If not installed, go back and install Git.


# 3. Create a Project Folder
You can create any folder. 

Example:
mkdir my-first-project

Go inside it:
cd my-first-project

Right now, this is just a normal folder — NOT a Git repo yet.


# 4. Initialize Git Repository
Inside the project folder, run:

git init

- This command creates a hidden folder named .git
- Your project is now officially a Git Repository

You will see:
Initialized empty Git repository in ...

- What Happened After git init?

Before git init → Normal folder
After git init → Git starts tracking changes


# 5. Check Repository Status
git status

You will see:

On branch master
No commits yet

This means Git is ready, but no files are added yet.


# 6. Create Your First File
You can create anything:

echo "Hello Git!" > demo.txt

Check status again:
git status

Now Git will show the file as Untracked.


# 7. Basic Git Workflow
This is the heart of Git.

- Step 1: Add file to staging
git add demo.txt

- Step 2: Commit it
git commit -m "My first commit"

 This saves your changes permanently in Git history.


# 8. View Commit History
git log

You’ll see your first commit details.


# Summary Table

| Action           | Command                   |
| ---------------- | ------------------------- |
| Check version    | `git --version`           |
| Create folder    | `mkdir folder-name`       |
| Go inside folder | `cd folder-name`          |
| Initialize Git   | `git init`                |
| Check status     | `git status`              |
| Add file         | `git add filename`        |
| Commit changes   | `git commit -m "message"` |
| View history     | `git log`                 |
