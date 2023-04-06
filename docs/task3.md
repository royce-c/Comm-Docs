# How to work with branches on github?
## Introduction
 One of the most important features of version control systems like Git and GitHub is the ability to create and manage branches. Branches allow you to work on multiple versions of your code simultaneously and keep your work organized.

Here are the 7 steps to create a new branch, make changes, and push those changes to GitHub:

## Step 1: Clone the repository

Use the git clone command to clone the repository to your local machine.

`git clone https://github.com/username/repository.git`

## Step 2: Create a new branch

 Use the git branch command to create a new branch.

 `git branch new-branch`

## Step 3: Switch to the new branch

Use the git checkout command to switch to the new branch.

`git checkout new-branch`

## Step 4: Make changes: Make the necessary changes to your code

## Step 5: Add changes to the staging area

Use the git add command to add the changes to the staging area.

`git add .`

## Step 6: Commit changes

Use the git commit command to commit the changes to the new branch.

`git commit -m "your commit message"`

## Step 7: Push changes to GitHub

Use the git push command to push the changes to the new branch on GitHub.

`git push -u origin new-branch`
