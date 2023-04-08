# How to push code to Github

## Introduction
In this guide we will be explaining how to push code to github. What this means is we be sending out code stored on our computers to a remote location (Github's servers) to be stored. Once our code is in Github's servers, github will host our code so others can view it and collaborate with us. Having code stored remotely is very useful because it can also serve as a backup incase our local repo is lost or corrupted.

Pushing code to Github is a crucial part of version control and collaboration for software development projects. This part of the documentation will guide you through the process of pushing your code to Github using the Git command-line interface and Visual Studio Code (VScode) text editor.

Before you begin, it is assumed that you have created a Github account and have an existing project that you want to push to Github. Additionally, you should have a basic understanding of Git commands and how to navigate through the terminal.
So let's get started and learn how to push your code to Github using Git and VScode!

## Step 1 - Launch vscode and open your project

Launch vscode and open your project that is not currently a git repository.

## Step 2 - Open directory in the integrated terminal and verify git installation

Open the terminal. You can do this via the keyboard shortcut via ``` ctrl ` ```

Verify you are in the correct directory by using the command `pwd`, this will print the working directory you are in. Make sure this is the folder returned to the terminal is the one you want to push to Github

Enter the command `git --version` this will return the version of git to the terminal. Do this to confirm git is installed correctly.

## Step 3 - Initialize git

Enter the command `git init`
This command initializes your folder by having git track changes.

To verify enter the command `ls -a`. This command lists all the files in your directory. If Git was initialized correctly than you should see a folder named .git in your directory.

Warning make sure you are in the correct directory before initializing git. If you initialize git in the wrong directory you will have to delete the .git folder from it and switch to the correct folder to restart.

## Step 4 - Add files to be staged

Enter the command `git add .`
The . character tells git to add all files in the folder. Alternatively, you could type each file you wish to add manually.

This command stages each of your files, what this means is git has added all the files in your folder to be committed.

To verify that it worked you can enter the command `git status` this will return the current status of Git. If it ran successfully you should see all the files that are staged to be committed printed in green on the terminal.

## Step 5 - Commit changes to local repository

Enter the command `git commit -m “<message>”` and replace <message> with your own message (do not include the <> characters around your message).

What this command does is commit your staged changes to your local repository.

## Step 6 - Add remote repository address

On github do this to obtain the url of your repo
This is known as the remote url because github is the remote location.
Enter the command `git remote add origin <REMOTE_URL>`

To verify enter `git remote -v` to view the remote repo

## Step 7 - Push to remote repository (github)

Enter the command `git push origin main`
This command pushes your local repo to the remote github repo.
Origin tells git where to push your code (in this case we set it as github)

## Conclusion

In conclusion, pushing code to Github is a fundamental aspect of version control and collaboration in software development projects. By following the steps outlined in this documentation, you can push your code to Github using Git and VScode. It is important to note that before starting, you need to have a Github account, an existing project that you want to push to Github, and a basic understanding of Git commands and navigating through the terminal. By initializing Git, adding files to be staged, committing changes to the local repository, adding the remote repository address, and finally pushing the local repository to the remote Github repository, you can ensure that your project is up to date and collaborative efforts are efficient.
