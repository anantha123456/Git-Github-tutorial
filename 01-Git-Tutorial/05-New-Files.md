### 05 – Working with New Files in Git


# 1. What Does “New File” Mean in Git?

A new file is any file created in your project directory that Git is not yet tracking.

- Git doesn’t automatically track files.
- You must manually add them to Git.


# 2. Create a New File

- Method 1: Using Terminal
echo "Hello Git!" > demo.txt

- Method 2: Using a Text Editor
Create a file manually:
demo.txt

- At this stage, Git sees it as Untracked.


# 3. Check Git Status
git status

- Expected Output:
File shown in red
Marked as Untracked

- Meaning: Git knows the file exists but is NOT tracking it.


# 4. Tell Git to Track the File (Staging)
git add demo.txt

- Now the file moves to the Staging Area.

 Verify Again:
git status

- File will appear in green
- Meaning: Ready to commit


# 5. Commit the New File
git commit -m "Added demo.txt file"

- This creates a snapshot of the file in Git history.


# 6. Confirm Commit
git log

You’ll see:
Commit ID
Author
Message
Date


# 7. Add Multiple New Files
git add file1.txt file2.txt file3.txt
Or add ALL new files:
git add .

# Be careful — git add . stages EVERYTHING.


# 8. Common Commands Summary
| Action          | Command                   |
| --------------- | ------------------------- |
| Create file     | `echo "text" > file.txt`  |
| Check status    | `git status`              |
| Stage file      | `git add <file>`          |
| Stage all files | `git add .`               |
| Commit changes  | `git commit -m "message"` |
| View history    | `git log`                 |


# 9. Git File Lifecycle
Untracked ➜ Staged ➜ Committed

- New file starts as Untracked
- After git add → Staged
- After git commit → Committed


## Quick Example
mkdir sample-project
cd sample-project
git init
echo "Sample file" > note.txt
git status
git add note.txt
git commit -m "Added note.txt"
git log



| Step | Command                          | Meaning               |

| 1    | `mkdir sample-project`           | Create project folder |
| 2    | `cd sample-project`              | Go inside folder      |
| 3    | `git init`                       | Start Git repo        |
| 4    | `echo "Sample File" > note.txt`  | Create a new file     |
| 5    | `git status`                     | Check file status     |
| 6    | `git add note.txt`               | Track file            |
| 7    | `git commit -m "Added note.txt"` | Save changes          |
| 8    | `git log`                        | View commit history   |

