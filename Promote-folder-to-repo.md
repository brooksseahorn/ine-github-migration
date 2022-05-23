# GitHub: Turning a folder into a repo

[TOC]

## Intro

This brief set of instructions describes how to take a pre-existing folder in a GitHub repo and turn it into its own repo.  I'll be using a concrete example based on the following structure:

```
|- Cloud team 

|-|- Brooks

|-|- Keith-Folder 

|-|- Melissa

|-|- Mike
```



We will be migrating the **Brooks** folder to the repo level.  This will be our target folder for these instructions.  Replace the example folder name (Brooks) with the folder you want to repo in the instructions.



## Clone the current repo

First, we need to get a copy of the folder that will become a repo.  We will clone down the repo that currently contains the target folder to do this.  Follow whatever process you clone directories with now.  

If you do not know how to clone a repo, stop here and get help from the team.

## Create the new repo on GitHub

Next, create a new repo in GitHub with the target folder's name.  In this example, this will be the **Brooks** folder.

1. On GitHub, in the **ine-content** organization, create a new repo with the desired name.  (*Note: Click the green **New** button.*)
2. In the **Repository name** field, type the name of the new repo (it will be the target folder's name).  
3. Enter a good description.
4. Change the visibility from **Public** to **Private**.
5. Click the **Create repository** button at the bottom of the page.



## Copy the command lines for creating a local repository

After clicking **Create repository**, the next page will display the instructions for setting up the repository on your local computer.  We want to copy the instructions under **…or create a new repository on the command line**.  Click the copy button at the top left of the box (see below).

![Initialize the local directory](https://github.com/brooksseahorn/ine-github-migration/blob/main/images/init_local_repo.png)

## Initialize the target folder

In a terminal, navigate to the target folder on your local machine and run the commands from above.  This will turn the folder into a source for your new GitHub repo.  However, only the file **README.md** will be pushed to GitHub.  Run a new commit as follows to add all the local folder's contents to the repo

```
git add .
git commit -m "Adding folders contents to rep."
git push
```



## Cleanup and finalize the local directory.

Now, we have a bit of a problem to resolve.  After following the above steps, we have a local repo in a local repo.  To fix this, clone the new GitHub repo at a top-level in your working directory.  You now have a new local directory and a new GitHub repo with this done.  You can archive or delete the local repo that was the source of the folder you promoted to a repo.

