### 13. Git Merge

# What is Merge?
Merge is used to combine changes from one branch into another branch.

Example:
You worked in a feature branch, and now you want those changes in main branch → use merge.


# When do we use Merge?

- When a task is completed in another branch
- To bring branch changes into main/master
- To update your branch with latest code


## Steps to Merge

# Step 1: Go to the branch where you want changes
Example: You want changes into main

git checkout main

# Step 2: Merge another branch into main
Example: Merge feature1 into main

git merge feature1

- Now main has feature1's changes.


# Types of Merge Results
- 1. Fast-Forward Merge
Happens when no other changes exist in main.

git merge feature1

- Simple
- No conflicts

- 2. Merge Conflict
Happens when both branches changed the same lines.

Git will show:
CONFLICT

- Fix the file manually
- Then run:
git add .
git commit -m "Resolved merge conflict"

# Check Merge Status
git log --oneline --graph


# Simple Real Example
You create a branch:

git checkout -b login-feature

You do some work and commit:

git add .
git commit -m "Added login page"

Now merge into main:

git checkout main
git merge login-feature

- Login feature added into main!

# Summary

| Action         | Command                                |
| -------------- | -------------------------------------- |
| Switch to main | `git checkout main`                    |
| Merge branch   | `git merge <branch>`                   |
| Fix conflict   | Edit file → `git add .` → `git commit` |
| View history   | `git log --oneline --graph`            |
