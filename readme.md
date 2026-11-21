# Git assignment

**Name:** Alicja Kawęcka  
**Date:** 21 November 2026  
**Course:** Basic Toolkit  
**Field of study:** Bioinformatics

## Description

This repository was created as part of an assignment to practice using Git and GitHub.  
The purpose of this project is to learn basic Git commands, version control, and how to manage changes in a repository.

## Basic Information about Git

Git is a version control system that allows users to track changes in their projects, save different versions of files, and collaborate with other people. GitHub is an online platform used to store and share Git repositories.

## Basic Git commands
### Configuration
- `git config --global user.name "Your Name"` – sets the author's name.  

- `git config --global user.email "your@email.com"` – sets the author's email address.

### Creating and Managing Repositories
- `git clone <repository_URL>` – creates a local copy of a repository.  
- `git status` – shows the current status of the repository.  
- `git log --oneline` – displays a short history of commits.

### Saving Changes
- `git add <file_name>` – stages a selected file for the next commit.  
- `git add .` – stages changes in the current directory and its subdirectories.  
- `git add -u` – stages modified and deleted tracked files, but not new files.  
- `git commit -m "message"` – saves staged changes with a descriptive message.  
- `git commit --amend -m "new message"` – changes the most recent commit message.

### Working with GitHub
- `git push` – uploads local commits to the remote repository.  
- `git pull` – downloads and integrates changes from the remote repository.  
- `git fetch` – downloads information about remote changes without merging them into the current branch.

### Branching and Merging
Branches allow users to experiment with different versions of a project without changing the main branch.  
- `git branch` – lists local branches.  
- `git branch new_branch` – creates a new branch.  
- `git checkout new_branch` – switches to an existing branch.  
- `git checkout -b new_branch` – creates and switches to a new branch.  
- `git merge new_branch` – merges changes from another branch into the current branch.  
- `git diff main..new_branch` – compares the contents of two branches.

## Merge Conflicts
A merge conflict can occur when different branches modify the same part of a file. Git cannot automatically decide which version should be kept.  
To resolve a conflict:  
1. Open the file containing the conflict.  
2. Find the conflict markers (`<<<<<<<`, `=======`, `>>>>>>>`).  
3. Choose the correct version or combine both versions.  
4. Remove the conflict markers and save the file.  
5. Use `git add <file_name>` and `git commit` to finish the merge.

## Pulling Changes
`git pull` is used to update local files with changes from a remote repository (GitHub). It is especially useful when working on the same project on different computers or collaborating with other people.  
### How to Pull Changes
1. Clone the repository on another computer:  
`git clone <repository_URL>`. 
2. Modify the files, commit the changes and push them to GitHub:  
`git add .`  
`git commit -m "new changes"`  
`git push origin main`  
3. Return to the first computer and download the changes:  
`git pull`

### Pull Conflicts
Conflicts may occur when the same parts of a file are modified independently on different computers or branches.  
- `git fetch` – downloads information about remote changes without modifying local files.
- `git merge origin/main` – attempts to merge the remote changes into the current branch.  
- `git status` – shows which files contain unresolved conflicts.  

If a conflict occurs, we need to open the file, choose which changes to keep, remove the conflict markers and save the file.  

Finally, we can use:  
1. `git add <file_name>` – stages the resolved file.  
2. `git commit -m "resolve merge conflict"` – saves the resolution.  
3.  `git push` – uploads the merged changes to GitHub.

## Why Is Git Useful?
Git helps organize projects, track changes, and recover previous versions of files. It is especially useful in scientific research because it supports reproducibility, documentation, and collaboration between researchers.