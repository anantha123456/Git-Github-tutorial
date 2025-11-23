### 02-Creating-Remote-Repo

# What is a Remote Repository?
A remote repo is a Git repository stored on GitHub (online).
It allows you to store code online, collaborate, and share projects.

# 1. Login to GitHub
Open: https://github.com
Sign in with your account.

# 2. Create a New Repository

1. Click New or + → New repository
2. Enter:
- Repository Name (example: my-first-repo)
- Description (optional)
3. Select:
Public ✅
4. Keep these unchecked
- Add README
- .gitignore
- License
5. Click Create repository

# 3. Copy the Repo URL
You'll see two URLs:
- HTTPS (Recommended)
https://github.com/username/my-first-repo.git

Copy this URL.

# 4. Connect Local Repo to GitHub
Go to your local project folder in terminal:
git remote add origin https://github.com/username/my-first-repo.git

Verify:

git remote -v

# 5. Push Code to GitHub

If you already have commits:

git branch -M main
git push -u origin main

Now your project is uploaded.

# Summary

| Step | Action             |
| ---- | ------------------ |
| 1    | Login GitHub       |
| 2    | Create repository  |
| 3    | Copy URL           |
| 4    | Connect local repo |
| 5    | Push code          |

# Troubleshooting

# Error: "not a git repository"
- Solution:
git init

# Error: "nothing to commit"
- Solution: Add a file and commit:

echo "Hello" > demo.txt
git add demo.txt
git commit -m "First commit"
