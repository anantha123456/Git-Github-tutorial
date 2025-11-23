### 02-Switch-Branches


## What Does “Switch Branch” Mean?
Switching branches means moving from one workspace to another.

Example:
- You are on main
- You switch to feature-ui
- Now you are working in that branch only.


# 1. Check Current Branch
git branch

- The branch with * is your current branch.


# 2. Switch to an Existing Branch
git checkout <branch-name>

Example:
git checkout feature-ui

- Now you're inside feature-ui


# 3. Switch Back to Main
git checkout main


# 4. New Command (Latest Git Recommended)
You can use switch instead of checkout:

Switch to a branch:
git switch <branch-name>

Example:
git switch feature-ui


# 5. If the Branch Doesn't Exist
You’ll get an error.

Create + switch:
git checkout -b <branch-name>

Example:
git checkout -b feature-backend


# 6. Warning 
If you have uncommitted changes, Git may block switching.

Fix:

git add .
git commit -m "Saved work"

Then switch:
git checkout <branch>


# Summary Table

| Action             | Command                  |
| ------------------ | ------------------------ |
| See current branch | `git branch`             |
| Switch branches    | `git checkout <name>`    |
| Recommended switch | `git switch <name>`      |
| Create + switch    | `git checkout -b <name>` |
