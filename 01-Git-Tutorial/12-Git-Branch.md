### 12 - Git Branch 

# What is a Branch?
A branch is like a separate workspace.

- You can do changes
- Without affecting the main code
- Main branch = master or main

# 1. See Current Branch
git branch
- The branch with * is your current branch.

# 2. Create a New Branch
git branch dev
- Creates a branch named dev

# 3. Switch to a Branch
git checkout dev
- Moves you to dev branch

# 4. Create + Switch (Shortcut)
git checkout -b dev

- Creates dev
- Switches to dev

# 5. Delete a Branch
git branch -d dev

- Deletes the branch (only if merged)

Force delete:
git branch -D dev

# 6. Rename a Branch
git branch -m newname

# 7. See Remote + Local Branches
git branch -a

# Quick Summary

| Action          | Command               |
| --------------- | --------------------- |
| See branches    | `git branch`          |
| Create branch   | `git branch dev`      |
| Switch          | `git checkout dev`    |
| Create + switch | `git checkout -b dev` |
| Delete          | `git branch -d dev`   |

# One Line Memory Trick
- branch = separate workspace