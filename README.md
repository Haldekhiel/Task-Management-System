
Simple Task Management System Using Git

Project Description

This project creates a task management system using a text file in a Git repository, applying key Git concepts such as branching, merging, and rebasing.
Project Requirements

# Set Up the Repository

git init task-manager
cd task-manager
touch tasks.txt
* Initializes a Git repository and creates tasks.txt.

# Add Initial Tasks

echo "- Learn Git basics" >> tasks.txt
echo "- Set up Git repository" >> tasks.txt
git add tasks.txt
git commit -m "Add initial tasks"
* Adds initial tasks and commits them.
# Create Branches and Work on Features

git checkout -b feature/add-tasks
# Add more tasks
git add tasks.txt
git commit -m "Add more tasks"

git checkout -b feature/remove-tasks
# Remove a task
git add tasks.txt
git commit -m "Remove a task"
* Creates branches for adding and removing tasks, then commits changes.
4. Merge Branches and Handle Conflicts

git checkout master
git merge feature/add-tasks
git merge feature/remove-tasks
# Resolve conflicts in tasks.txt
git add tasks.txt
git commit -m "Resolve merge conflicts"
* Merges branches and resolves any conflicts.
5. Use Git Rebase

git checkout -b feature/update-tasks
# Update tasks
git add tasks.txt
git commit -m "Update tasks"
git checkout master
git rebase feature/update-tasks
* Rebases changes from the update tasks branch onto master.
6. Reverting to Previous Commits

echo "- Some incorrect task" >> tasks.txt
git add tasks.txt
git commit -m "Add incorrect task"
git revert HEAD
* Reverts the last commit to undo changes.
7. Working with Remote Repository

git remote add origin https://github.com/Haldekhiel/Task-Management-System.git
git push -u origin master
* Links the local repository to GitHub and pushes changes.

# Task-Management-System
