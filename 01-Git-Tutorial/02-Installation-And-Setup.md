### Installation and Setup

# What You Will Learn
In this section, you will learn:

1. How to install Git
2. How to verify installation
3. How to configure Git for the first time
4. Basic setup on Windows & Linux


# 1. What is Needed Before Installation?

- Requirements

Laptop (Windows/Linux)
Internet Connection
Git Installer


# 2. Download Git

 Official Website (Homepage)
 https://git-scm.com/

Direct Download Page
https://git-scm.com/downloads


# 3. Install Git on Windows Step-by-Step

1. Go to the Git download page
2. Click "Download for Windows"
3. Run the installer
4. Keep all default options
5. Click Next → Next → Install
6. Finish installation


# 4. Install Git on Linux Ubuntu / Debian
 Open WSL Terminal

sudo apt update
sudo apt install git -y

# CentOS / RHEL / Fedora
sudo yum install git -y


# 5. Verify Installation
Run this command:

git --version

- Expected Output:

git version X.X.X


# 6. First-Time Git Configuration
Set your name:
git config --global user.name "Your Name"

Set your email:
git config --global user.email "your-email@example.com"

Check config:
git config --list


# 7. Optional Setup (Recommended) Default Editor Setup (VS Code)
git config --global core.editor "code --wait"


# 8. Summary
Step	Action
1	Download Git
2	Install Git
3	Verify Git
4	Configure Name & Email
5	Check Config


# Screenshots go here:

Git-GitHub-Course/assets/screenshots/

