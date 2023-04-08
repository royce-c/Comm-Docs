# How to use Git Stash?

## Introduction

In Git and GitHub, **"stashing"** refers to a feature that allows you to temporarily save changes that you have made to your working directory and index, without committing them to your Git repository.

Stashing is useful when you are in the middle of working on a feature or bugfix, and need to switch to a different branch or work on a different task. Instead of committing your changes and switching branches, you can stash your changes and then switch branches. Later, you can unstash your changes and continue working on them.

## Step 1: Check your current Git status

Before stashing changes, you should check the current status of your Git repository. Use the following command to check if you have any changes that are not yet committed:
`git status`

## Step 2: Stash your changes

Once you have confirmed that there are changes that you want to stash, you can use the following command to stash them:

`git stash save "Your stash message`

This will save your changes to a new stash with a message that you specify.

## Step 3: Check your Git stash list

After stashing changes, you can check the list of stashes you have created with the following command:

`git stash list` 

This will show you the stash ID and message for each stash.

## Step 4: Apply a stash

If you want to apply a stash, you can use the following command:

`git stash apply stash@{n}1`

Replace n with the index of the stash you want to apply. If you do not specify a stash index, the most recent stash will be applied.

## Step 5: Delete a stash

If you want to delete a stash, you can use the following command:

`git stash drop stash@{n}`

Replace n with the index of the stash you want to delete.

## Step 6: Apply and delete a stash

If you want to apply and delete a stash in one step, you can use the following command:

`git stash pop stash@{n}`

Replace n with the index of the stash you want to apply and delete

## Step 7: Clear all stashes

If you want to clear all stashes from your Git repository, you can use the following command:

`git stash clear`

This will delete all stashes permanently.

## Conclusion

In conclusion, stashing in Git is a powerful feature that enables you to temporarily save your changes without committing them. This is helpful when you need to switch to a different branch or work on a different task without losing your progress. In this guide, we have walked through the steps of how to stash changes, check the stash list, apply, delete, and clear all stashes. By mastering the stash command, you can streamline your Git workflow and work more efficiently on your projects.
