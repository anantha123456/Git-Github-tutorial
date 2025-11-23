### 05 - Feature Branch Workflow 
Feature Branch Workflow is a way to work on new features without touching the main branch until the work is complete.

# Why Use Feature Branch Workflow?

- Keeps main clean and stable
- Each feature is separate
- Avoids conflicts
- Easy teamwork

## Simple Workflow Steps

# 1. Start from main

Make sure your main branch is up to date.

git checkout main
git pull

# 2. Create a Feature Branch
git checkout -b feature-login

- Branch name format:

feature-login
feature-payment
feature-ui-update

# 3. Do Your Work
Modify files, add code, etc.

# 4. Stage & Commit Changes
git add .
git commit -m "Added login feature"

# 5. Push Feature Branch to GitHub
git push -u origin feature-login

# 6. Create a Pull Request (PR)
- On GitHub:

Compare feature-login → main
Review changes
Approve & Merge

# 7. Merge to main
After PR approval, merge the branch into main.
- Now main has the new feature.

# 8. Delete the Feature Branch
git branch -d feature-login
git push origin --delete feature-login

# Quick Summary Flow
main → create feature branch → code → commit → push → pull request → merge → delete branch


## Real Example
git checkout main
git pull
git checkout -b feature-login
# code work...
git add .
git commit -m "login ui added"
git push -u origin feature-login
# PR & merge
git branch -d feature-login
git push origin --delete feature-login


# When to Use This?

- New feature
- Bug fix
- UI change
- Big update


### Feature Branch Workflow Summary

# Update main
git checkout main
git pull

# Create feature branch
git checkout -b feature-login

# Work + Commit
git add .
git commit -m "Added login UI"

# Push branch
git push -u origin feature-login

# Create Pull Request

# Merge to main

# Delete branch
git branch -d feature-login
git push origin --delete feature-login
