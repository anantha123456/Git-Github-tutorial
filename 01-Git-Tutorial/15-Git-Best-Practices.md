### 15. Git Best Practices 

# 1. Don’t work on main
Always create a branch.

git checkout -b my-branch

# 2. Commit small changes
Small changes = easy to understand.

# 3. Write clear messages
- "Added login page"
- "stuff fixed"

# 4. Pull before push
git pull
git push

Avoids conflicts.

# 5. Use good branch names
- feature-login
- test123

# 6. Delete branch after merge
git branch -d my-branch

# 7. Don’t commit passwords or secrets
Never upload .env, keys, passwords.

# 8. Use .gitignore
To skip unwanted files.

# Summary in 5 words:
Branch – Commit – Message – Pull – Clean

Done.