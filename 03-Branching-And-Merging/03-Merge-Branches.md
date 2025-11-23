### 03 - Merge Branches


# What is Merging?

Merging means combining the changes from one branch into another.
Mostly, we merge feature branches into the main branch.

Example:
feature- login-page  →  main


# 1. Merge a Branch into Main
- Step 1: Switch to the branch you want to merge INTO

Usually main.

git checkout main

- Step 2: Pull latest changes (VERY IMPORTANT)
git pull origin main

- Step 3: Merge the branch
git merge feature-login

- If no conflicts → You will see:
Fast-forward
or
Merge made successfully

- Step 4: Push merged code to GitHub
git push origin main

- Now the feature branch code is inside main.


# 2. Merge Using GitHub (GUI Method)
- Push your branch to GitHub
- Open repo → Click Pull Requests
- Click New Pull Request
- Select:
Base branch = main
Compare branch = your feature branch
- Click Create Pull Request
- Click Merge Pull Request
- Delete branch (optional but recommended)


# 3. What Happens Internally?
- Git finds the last common commit between the two branches
- Combines changes
- Creates a new merge commit (if not fast-forward)
- Updates branch history


# 4. Merge Conflicts 
Conflicts happen when two branches change the same line in a file.

Example conflict:

<<<<<<< main
print("Hello from main")
=======
print("Hello from feature")
>>>>>>> feature-login

# How to Fix
- Open the file
- Edit manually to keep correct code
- Save
- Add the file
git add filename.py
- Commit
git commit -m "Resolved merge conflict"
- Then push:
git push origin main


# 5. Delete Branch After Merge (Optional but Best Practice)
git branch -d feature-login

If branch is already pushed to GitHub:

git push origin --delete feature-login


# Why delete?
- Code is already merged
- Keeps repo clean


# Summary Table

| Task                 | Command                                  |
| -------------------- | ---------------------------------------- |
| Switch to main       | `git checkout main`                      |
| Pull latest code     | `git pull origin main`                   |
| Merge branch         | `git merge feature-login`                |
| Push to GitHub       | `git push origin main`                   |
| Delete local branch  | `git branch -d feature-login`            |
| Delete remote branch | `git push origin --delete feature-login` |


# Real-Life Example
You create a branch:
git checkout -b feature-payment

Work → Commit → Push

Then merge:

git checkout main
git pull origin main
git merge feature-payment
git push origin main

---- Payment feature successfully merged into main!