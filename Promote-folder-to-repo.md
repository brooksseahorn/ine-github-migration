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



## Clone the current repo

First, we need to get a copy of the folder that will become a repo.  To do this, we will clone down the repo that currently contains the repo.  Follow whatever process you clone directories with currently.  

If you are not familiar with cloning repos, here's what you do:

1. Log into GitHub and navigate to the target repo.

2. Once on the repo page, click the green 

3. Click the copy button to get a copy of the repo's URL.

   ![Clone URL](https://github.com/brooksseahorn/ine-github-migration/blob/main/images/clone-url.png)

4. From the command line of your operating system (where you have already installed git) run the following command:   

   ```bash
   git clone <<Paste the URL copied above here>>
   ```

   

## Create a repo on GitHub

Start off by creating a new repo in GitHub with the name of the target folder.  In this example, this will be the **Brooks** folder.

1. On GitHub, in the **ine-content** organization, create a new repo with the desired name.  (*Note: Click the green **New** button.*)
2. In the **Repository name** field type the name of the new repo.  
3. Enter a good description.
4. Change the visibility from **Public** to **Private**.
5. Click the **Create repository** button at the bottom of the page.



## Copy the command lines for creating a local repository

After clicking **Create repository** the next page will display the instructions for setting up the repository on your local computer.  We want to copy the instructions under **…or create a new repository on the command line**.  Click the copy button at the top left of the box (see below).

![Initialize the local directory](https://github.com/brooksseahorn/ine-github-migration/blob/main/images/init_local_repo.png)



