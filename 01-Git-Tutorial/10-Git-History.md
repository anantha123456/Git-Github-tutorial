### 10 - Git History

# Git history means:
 Seeing all the commits you made in the project.

# 1. See All Commits
git log

Shows:
Who committed
When
Message

# 2. Short & Clean History
git log --oneline

Example output:
7c9d2bf Added file
107c5fb First commit

# 3. See History of One File
git log file.txt

# 4. See Details of One Commit
git show <commit-id>

Example:
git show 7c9d2bf

# 5. Compare Two Commits
git diff <id1> <id2>


# Small Summary

| What you want  | Command             |
| -------------- | ------------------- |
| Full history   | `git log`           |
| Short history  | `git log --oneline` |
| File history   | `git log file.txt`  |
| Commit details | `git show <id>`     |

# One Line Memory Trick
- log = history
- show = details
- diff = compare