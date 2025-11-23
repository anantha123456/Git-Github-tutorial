### 14. Git Workflow

# What is Git Workflow?
It is the step-by-step process of how we work with Git from starting a project to updating code.

Simple meaning:
- How code moves from your laptop to the main project.

# Basic Git Workflow (Most Common)
# 1. Create / Clone a Repository
If new project:

git init

If project already exists on GitHub:

git clone <repo-url>

# 2. Create a Branch
We don’t work directly on main.

git checkout -b feature1

# 3. Do Changes

Write code, edit files, etc.

# 4. Add Changes
git add .

# 5. Commit Changes
git commit -m "Added new feature"

# 6. Push to Remote (GitHub)
git push origin feature1

# 7. Create Pull Request (PR)

Done on GitHub

Request to merge feature1 into main

Team reviews the code

# 8. Merge into main

After approval:

git checkout main
git merge feature1

# 9. Update Local main
git pull origin main

# Simple Workflow Diagram
Clone/Init → Create Branch → Add → Commit → Push → Pull Request → Merge → Update main

# Why Workflow is Important?
- Safe
- Organized
- No code loss
- Team-friendly

# Very Short Summary

| Step | Action        | Command                   |
| ---- | ------------- | ------------------------- |
| 1    | Create/Clone  | `git init` / `git clone`  |
| 2    | Create branch | `git checkout -b feature` |
| 3    | Add changes   | `git add .`               |
| 4    | Commit        | `git commit -m "msg"`     |
| 5    | Push          | `git push origin feature` |
| 6    | Merge         | `git merge feature`       |
| 7    | Update main   | `git pull`                |
