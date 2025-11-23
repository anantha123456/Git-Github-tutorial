### 09. Git Stash 


# What is Stash?
- Temporary save for your changes.
- Use it when your work is not complete and you don’t want to commit.

# 1. Save Your Changes
git stash

- Your changes are saved
- Your working directory becomes clean

# 2. See Saved Stashes
git stash list

# 3. Bring Back Your Changes
git stash pop

- Restores changes
- Removes stash from list

# 4. If You Want to Keep Stash (Don’t Delete)
git stash apply

- Restores changes
- Does NOT delete stash

# 5. Delete All Stashes
git stash clear


# Simple Real-Life Example

You are working on a file and suddenly need to switch branch:

git stash
git checkout dev

After work:

git checkout master
git stash pop

- Your work comes back!


# Remember in 5 Seconds

| Action           | Command           |
| ---------------- | ----------------- |
| Save changes     | `git stash`       |
| Show stash list  | `git stash list`  |
| Restore & delete | `git stash pop`   |
| Restore only     | `git stash apply` |
| Delete all       | `git stash clear` |
