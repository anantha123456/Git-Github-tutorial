### 16. Git Basic Commands
These are the MOST used Git commands.

# 1. Check Git Version
git --version

# 2. Initialize Git in a Folder
(Starts Git tracking)

git init

# 3. Check File Status
(See new/modified files)

git status

# 4. Add Files to Staging

git add file.txt
Add all files:
git add .

# 5. Commit Files
(Save changes)

git commit -m "Your message"

# 6. View Commit History

git log
Simple history:
git log --oneline

# 7. Create a Branch
git branch my-branch

# 8. Switch to Branch
git checkout my-branch

# 9. Create & Switch in One Step
git checkout -b my-branch

# 10. Merge Branch into Main
git checkout main
git merge my-branch

# 11. Delete Branch
git branch -d my-branch

# 12. Add Remote Repo (GitHub)
git remote add origin <repo-url>

# 13. Push Code to GitHub
git push origin main

# 14. Pull Latest Code
git pull origin main

# 15. Clone a Repo
git clone <repo-url>

## Quick Summary

| Action       | Command               |
| ------------ | --------------------- |
| Start Git    | `git init`            |
| Add files    | `git add .`           |
| Commit       | `git commit -m "msg"` |
| Check status | `git status`          |
| Push         | `git push`            |
| Pull         | `git pull`            |



### Git Basic Commands – Quick List

# Setup
git --version
git config --global user.name "Your Name"
git config --global user.email "you@example.com"

# Initialize Repo
git init

# File Status
git status

# Staging Files
git add file.txt
git add .

# Commit
git commit -m "message"

# History
git log
git log --oneline

# Branching
git branch
git branch my-branch
git checkout my-branch
git checkout -b my-branch
git branch -d my-branch

# Merging
git checkout main
git merge my-branch

# Remote (GitHub)
git remote add origin <repo-url>
git remote -v

# Push & Pull
git push origin main
git pull origin main

# Clone
git clone <repo-url>