# Using Git LFS for Large Files
[![Medium](https://img.shields.io/badge/Medium-Read%20Article-green?logo=medium&style=for-the-badge)](https://medium.com/@ArunKarthikPeriyaswamy/how-to-easily-push-large-files-to-github-using-git-lfs-7aa70fba03cc)

## Introduction
Git LFS (Large File Storage) is an extension that helps manage large files in your Git repositories. Follow these steps to use Git LFS effectively:

## Prerequisites
Make sure you have Git and Git LFS installed on your system.

### Step 1: Install Git LFS

# For macOS with Homebrew
brew install git-lfs

# For Debian-based Linux
sudo apt-get install git-lfs

Step 2: Configure Git LFS
Run this command to configure Git LFS:
git lfs install

Step 3: Specify Large Files
Create a .gitattributes file in your repository and add the following line to track all .zip files:
*.zip filter=lfs diff=lfs merge=lfs -text

