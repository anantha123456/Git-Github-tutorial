### 01-Create-Branch


# What is a Branch?
A branch is like a separate workspace where you can make changes without affecting the main code.

 Example:
main branch = stable code
feature-login branch = your new feature work


# Why Create a Branch?

- Work safely without breaking main
- Develop new features
- Fix bugs separately
- Team collaboration


# 1. View Existing Branches
git branch


# 2. Create a New Branch
git branch <branch-name>

Example:
git branch feature-ui

This creates the branch but does not switch to it.


# 3. Create & Switch in One Command (Recommended )
git checkout -b <branch-name>

Example:
git checkout -b feature-ui

Now you're working inside that branch.


# 4. Switch Back to Main
git checkout main


# 5. Delete a Branch (After Merging)
git branch -d <branch-name>

Example:
git branch -d feature-ui


# Quick Workflow
git branch feature-ui
git checkout feature-ui
(work… commit…)
git checkout main

- Verify Current Branch
git branch

- The branch with * is your active branch.


# Summary Table

| Action          | Command                  |
| --------------- | ------------------------ |
| List branches   | `git branch`             |
| Create branch   | `git branch <name>`      |
| Create + Switch | `git checkout -b <name>` |
| Switch branch   | `git checkout <name>`    |
| Delete branch   | `git branch -d <name>`   |

