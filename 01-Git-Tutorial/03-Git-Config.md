### 03 – Git Config

## What is Git Config?

When you use Git, it needs to know:

- Who are you? (Your name)
- What is your email?

Because this information goes into every commit you make.

So Git Config = Telling Git your identity + preferences


## Why do we need it?

Because when you push code to GitHub, GitHub should show:
- Who wrote the code
- Who made the commit
- Who contributed

Without this, Git will give errors.


## Types of Git Config Levels

| Level      | Meaning                 | Scope            | File Location    |
| ---------- | ----------------------- | ---------------- | ---------------- |
| **System** | Applies to all users    | Entire system    | `/etc/gitconfig` |
| **Global** | Applies to current user | User account     | `~/.gitconfig`   |
| **Local**  | Applies to one repo     | Specific project | `.git/config`    |

-Priority Order (Highest to Lowest):
Local → Global → System


# Step 1: Open Terminal

If you're on Windows:
- Open Git Bash

If you're on Linux:
- Open Terminal

# Step 2: Set Your Name

Type this 
git config --global user.name "Your Name"

Example:
git config --global user.name "Anantha Lakshmi"

This tells Git your name.

# Step 3: Set Your Email

git config --global user.email "yourmail@gmail.com"

Example:
git config --global user.email "anantha@example.com"

This tells Git your email.

# Step 4: Check if it's saved

git config --list

You should see something like:

user.name=Anantha Lakshmi
user.email=anantha@example.com

- That means Git is ready!


# Simple Meaning

| Thing    | Why?                       |
| -------- | -------------------------- |
| Name     | To show who wrote the code |
| Email    | To track contributions     |
| --global | Apply to your whole laptop |


# You ONLY need to remember these 3 commands

git config --global user.name "Your Name"
git config --global user.email "yourmail@gmail.com"
git config --list

That's it.



