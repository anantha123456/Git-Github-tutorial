### 05-Cloning-Repo

# What is Cloning?
Cloning means downloading a GitHub repo to your local system so you can work on it.
It creates a full copy of the project including:

- Files
- Folders
- Commit history
- Branches

# When Do We Clone?
You clone when:

- You want to work on someone else's repo
- You want the repo on a new laptop
- You joined a team project

# Command to Clone
git clone <repo-url>

Example:
git clone https://github.com/anantha/sample-project.git

- This creates a folder named sample-project on your system.

# Steps to Clone a GitHub Repo

- Step 1: Go to GitHub Repo
Open the repository you want to download.

- Step 2: Click "Code" Button
You will see a URL.

- Step 3: Copy the HTTPS URL
Example:
https://github.com/user/repo.git

- Step 4: Open Terminal / Git Bash
Go to the folder where you want the repo.

cd Desktop

- Step 5: Run Clone Command
git clone <repo-url>

- Step 6: Enter Repo Folder
cd repo

- Now the project is ready to use.

# Clone with SSH (Optional)
If SSH key is set:

git clone git@github.com:user/repo.git

# Verify Clone
git remote -v

You should see origin pointing to GitHub.

# Summary

| Action           | Command           |
| ---------------- | ----------------- |
| Clone a repo     | `git clone <url>` |
| Move into folder | `cd <repo>`       |
| Check remote     | `git remote -v`   |
