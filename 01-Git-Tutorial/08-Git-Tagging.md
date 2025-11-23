### 08 - Git Tagging

# What is a Tag?
A tag is like a label for a specific commit.

We use tags to mark important points in a project, like:
- Version releases
- Milestones
- Stable checkpoints

Example:
v1.0
v2.5
release-1


# Types of Tags

# 1. Lightweight Tag
 Just a name pointing to a commit (no message, no metadata)
git tag v1.0

# 2. Annotated Tag
 Recommended : Includes message, author, date, commit info
git tag -a v1.0 -m "First project release"


# View Tags
git tag

List tags in order:
git tag --sort=taggerdate

# Tag a Specific Commit
If you want to tag an older commit:

Step 1: Get commit ID
git log --oneline

Step 2: Tag it
git tag -a v2.0 <commit-id> -m "Release v2.0"

Example:
git tag -a v2.0 3ab2cde -m "Second release"

# Delete a Tag
git tag -d v1.0


# Push Tags to Remote (GitHub)
Push one tag:
git push origin v1.0

Push all tags:
git push origin --tags


# Delete Tag from Remote
git push origin --delete v1.0


# Quick Example (Simple)
echo "Hello" > app.txt
git add app.txt
git commit -m "Added app.txt"

git tag -a v1.0 -m "First version"
git tag
git push origin v1.0

- Tag created
- Tag pushed


# When to Use Tags?

| Situation       | Use Tag? |
| --------------- | -------- |
| First release   |   Yes    |
| Stable version  |   Yes    |
| Bug fix version |   Yes    |
| Small changes   |   No     |



# Summary

| Command                    | Purpose                |
| -------------------------- | ---------------------- |
| `git tag`                  | List tags              |
| `git tag v1.0`             | Create lightweight tag |
| `git tag -a v1.0 -m "msg"` | Create annotated tag   |
| `git tag -d v1.0`          | Delete tag             |
| `git push origin v1.0`     | Push a tag             |
| `git push origin --tags`   | Push all tags          |


