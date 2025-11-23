### 04-Pushing-Code


# What is "Push"?
Push = Uploading your local code to GitHub (remote repo).
Local  → GitHub 

# 1. Make Sure You Are Inside Your Project
cd my-first-project

# 2. Check Status
git status

- Red files = Not tracked
- Green files = Ready to commit
- Nothing to commit = Clean

# 3. Add Files to Staging
git add .

# 4. Commit the Changes
git commit -m "Your message"

Example:
git commit -m "Added README file"

- Commit = Save locally.

# 5. Push to GitHub
First push:
git push -u origin main

Next pushes:
git push

- Now code is on GitHub 

# When Do We Push?

| Situation      | Action     |
| -------------- | ---------- |
| New file added | `git push` |
| Code updated   | `git push` |
| Bug fixed      | `git push` |
| After commit   | `git push` |

# Push Flow (Simple)
Write Code → git add → git commit → git push

# Common Errors & Fixes
- "No commits yet"
git add .
git commit -m "Initial commit"

- "origin not found"
git remote add origin <URL>

- "branch main not found"
git branch -M main

- Authentication failed
Login GitHub Desktop / Browser
Check username & token (if required)

# Verify Push
- Go to GitHub → Open repo → Refresh
- You should see your files.

# Quick Example
git add .
git commit -m "Updated code"
git push
