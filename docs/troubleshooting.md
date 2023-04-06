# Troubleshooting

## Pushing to github troubleshooting guide

### fatal: not a git repository (or any of the parent directories)

If you encounter this error, it means that you're not in the correct directory or you haven't initialized git yet. Double-check that you're in the correct directory and that you've initialized git using the git init command.

### remote: Repository not found

If you encounter this error, it means that the remote repository that you're trying to push to doesn't exist or that you've entered the wrong remote URL. Double-check that you've entered the correct remote URL and that the repository exists on GitHub. You can check the remote URLs using the command `git remote -v`.

### Updates were rejected because the remote contains work that you do not have locally

If you encounter this error, it means that the remote repository that you're trying to push to has changes that you don't have in your local repository. You'll need to pull the changes from the remote repository first using the git pull command before pushing your changes to the remote repository. For example, git pull origin main to pull changes from the remote repository before pushing your changes using git push origin main.

## Git stash troubleshooting guide

### git stash: Your local changes to the following files would be overwritten by merge

If you encounter this error when trying to apply a stash, it means that the changes in your stash conflict with changes that you've made locally. You can resolve the conflict by manually merging the changes or by discarding your local changes and applying the stash. To discard your local changes, you can use the following command:

`git reset --hard HEAD`

This will reset your working directory to the state of the last commit, discarding any changes that you've made.

### git stash: Cannot save the current index state

If you encounter this error when trying to stash changes, it means that you have changes in your index (staging area) that cannot be stashed. This can happen if you have conflicts or if you have added files to the index that are not tracked by git. To resolve this error, you can either commit your changes before stashing them or use the --include-untracked option with the `git stash` command to include untracked files in the stash.

### git stash: No stash found

If you encounter this error when trying to apply or delete a stash, it means that the stash you're trying to access doesn't exist. Double-check the stash ID or index that you're using and make sure that the stash hasn't been deleted.

### git stash: Failed to apply stash

If you encounter this error when trying to apply a stash, it means that there was a conflict while applying the stash. You can resolve the conflict manually by merging the changes or by discarding the stash and making the changes manually. To discard the stash, you can use the following command:

`git stash drop stash@{n}`

Replace n with the index of the stash that you want to drop.
