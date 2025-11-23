### 06 – Git Staging Area


# What is the Staging Area?
The staging area (also called index) is a place where Git collects the changes before committing them.

- Think of it like a shopping cart:
You edit files.
You add selected files to staging.
Then you commit them.

So staging allows you to choose which changes should go into the next commit.


# Workflow
Working Directory → Staging Area → Repository
   (edited files)     (git add)      (git commit)


## Important Commands

# 1. Check Status
Shows which files are tracked, untracked, staged, or modified.

git status

# 2. Add a Single File to Staging
git add filename


Example:
git add app.py

# 3. Add All Files to Staging
git add .
OR
git add -A

# 4. Add Specific File Types
git add *.txt

This adds all .txt files.

# 5. Remove a File From Staging (Unstage)
git restore --staged filename

Example:
git restore --staged app.py

# 6. View Staged Changes
git diff --staged


# Real-Time Example

Step 1: Create a file
echo "Hello Git" > demo.txt

Step 2: Check Status
git status

Step 3: Add to Staging
git add demo.txt

Step 4: Commit
git commit -m "Added demo file"


# Why Staging is Important?

- Allows selective commit
- Helps clean commit history
- Useful in teamwork
- Prevents accidental commits

Example:
You changed 5 files but want to commit only 2 → staging makes it possible.


# Summary

| Area              | Meaning               | Command      |
| ----------------- | --------------------- | ------------ |
| Working Directory | Files you edit        | —            |
| Staging Area      | Files ready to commit | `git add`    |
| Repository        | Saved commits         | `git commit` |


# Quick Commands Checklist

git status
git add filename
git add .
git restore --staged filename
git diff --staged