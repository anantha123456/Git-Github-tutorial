### 07 – Git Commit 


# What is a Commit?
A commit is like saving a version of your project.

- It stores:
What changed
Who changed it
When it changed


## Steps to Commit

# Step 1: Check status
git status

# Step 2: Add changes to staging
git add filename
or add everything:
git add .

# Step 3: Commit
git commit -m "Your message"

- Example:
git commit -m "Added login page"


# Useful Commands

| Purpose                    | Command                |
| -------------------------- | ---------------------- |
| Commit staged changes      | `git commit -m "msg"`  |
| Commit all tracked changes | `git commit -am "msg"` |
| Change last commit message | `git commit --amend`   |
| View commit history        | `git log`              |
| Short history              | `git log --oneline`    |


# Simple Real Example
mkdir test-project
cd test-project
git init
echo "Hello" > test.txt
git add test.txt
git commit -m "Added test file"
git Status
git log --oneline

- Good:
"Fixed dashboard bug"

- Bad:
"Changes"


# Simple Summary
git add .
git commit -m "message"
git log --oneline