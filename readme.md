# Git assignment

**Name:** Alicja Kawęcka  
**Date:** 21 November 2026  
**Course:** Basic Toolkit  
**Field of study:** Bioinformatics

## Description

This repository was created as part of an assignment to practice using Git and GitHub.  
The purpose of this project is to learn basic Git commands, version control, and how to manage changes in a repository.

## Git basic information

Git is a version control system that allows users to track changes in their projects, save different versions of files, and collaborate with other people. GitHub is an online platform used to store and share Git repositories.

## Basic Git commands
### Configuration
- `git config --global user.name "Your Name"` – sets the author's name.  

- `git config --global user.email "your@email.com"` – sets the author's email address.

###Creating and Managing Repositories
- `git clone <repository_URL>` – creates a local copy of a repository.  
- `git status` – shows the current status of the repository.  
- `git log --oneline` – displays a short history of commits.

###Saving Changes
- `git add <file_name>` – stages a selected file for the next commit.  
- `git add .` – stages changes in the current directory and its subdirectories.  
- `git add -u` – stages modified and deleted tracked files, but not new files.  
- `git commit -m "message"` – saves staged changes with a descriptive message.  
- `git commit --amend -m "new message"` – changes the most recent commit message.

###Working with GitHub
- `git push` – uploads local commits to the remote repository.  
- `git pull` – downloads and integrates changes from the remote repository.  
- `git fetch` – downloads information about remote changes without merging them into the current branch.

###Branching and Merging
Branches allow users to experiment with different versions of a project without changing the main branch.  
- `git branch` – lists local branches.  
- `git branch new_branch` – creates a new branch.  
- `git checkout new_branch` – switches to an existing branch.  
- `git checkout -b new_branch` – creates and switches to a new branch.  
- `git merge new_branch` – merges changes from another branch into the current branch.  
- `git diff main..new_branch` – compares the contents of two branches.

###Merge Conflicts
A merge conflict can occur when different branches modify the same part of a file. Git cannot automatically decide which version should be kept.  
To resolve a conflict:  
1. Open the file containing the conflict.  
2. Find the conflict markers (<<<<<<<, =======, >>>>>>>).  
3. Choose the correct version or combine both versions.  
4. Remove the conflict markers and save the file.  
5. Use git add <file_name> and git commit to finish the merge.

##Why Is Git Useful?
Git helps organize projects, track changes, and recover previous versions of files. It is especially useful in scientific research because it supports reproducibility, documentation, and collaboration between researchers.