### 03-Connecting-Local-To-GitHub

## What Does This Mean?

We are linking:
Local Repo (your laptop) , Remote Repo (GitHub)
So we can upload code online.


# 1. Go to Your Project Folder
Open terminal and navigate:
cd folder-name

- Example:
cd my-first-project

Make sure Git is initialized:

git init


# 2. Check If You Have a Commit
GitHub only accepts committed files.

Check:
git status

If untracked files exist:

git add .
git commit -m "Initial commit"


# 3. Add Remote GitHub URL
Copy your GitHub repo HTTPS URL:

Example:
https://github.com/username/my-first-repo.git

Connect it:
git remote add origin https://github.com/username/my-first-repo.git

- Verify:
git remote -v

You should see:

origin  https://github.com/username/my-first-repo.git (fetch)
origin  https://github.com/username/my-first-repo.git (push)


# 4. Push Code to GitHub
Rename branch to main (recommended):
git branch -M main

Push:
git push -u origin main

- Now your code is live on GitHub!


# 5. Make Next Changes & Push Again
After editing files:

git add .
git commit -m "Updated project"
git push

# Common Errors & Fixes

- Error: remote 'origin' already exists

- Fix:
git remote remove origin
git remote add origin https://github.com/username/repo.git


- Error: nothing to commit

- Fix:
Add or edit files first.

- Error: authentication failed

- Fix:
Login GitHub → Use HTTPS → Make sure you're signed in.


# Summary

| Step            | Command                          |
| --------------- | -------------------------------- |
| Initialize Repo | `git init`                       |
| Commit Files    | `git add .` + `git commit -m ""` |
| Add Remote      | `git remote add origin URL`      |
| Push Code       | `git push -u origin main`        |
