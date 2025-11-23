### 03-Merge-Conflicts

## Merge Conflicts

# What is a Merge Conflict?
When two people edit the same part of a file, Git doesn’t know which change is correct.

Example:
Two users edit Line 10 in app.js differently.

# When it Happens?
- During merge
- During pull
- During rebase

# Fixing Merge Conflicts

1. Open the file with conflict
You will see:

<<<<<<< HEAD
Your changes
=======
Other changes
>>>>>>> branch-name

2. Keep the correct content
3. Delete conflict markers
4. Add + Commit

git add .
git commit -m "Resolved merge conflict"