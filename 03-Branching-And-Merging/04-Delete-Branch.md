## 04 - Delete Branch 
When your work on a branch is finished and merged, you can delete it to keep things clean.


# 1. Delete Branch Locally (In your system)
git branch -d feature-login

Deletes the branch safely (only if merged).
  
- Force delete (if NOT merged)

git branch -D feature-login

 Careful! This removes the branch even if work is not merged.

 
 # 2. Delete Branch On GitHub (Remote)
git push origin --delete feature-login

- This removes the branch from GitHub.


# Quick Summary

| Action                      | Command                               |
| --------------------------- | ------------------------------------- |
| Delete local branch         | `git branch -d branchname`            |
| Force delete local          | `git branch -D branchname`            |
| Delete remote GitHub branch | `git push origin --delete branchname` |


# Example
Branch name: feature-login

git branch -d feature-login
git push origin --delete feature-login

---- Done! Branch removed locally and on GitHub.

