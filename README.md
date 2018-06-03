# Useful Git commands

- [Installing Git Software](#installing-git-software)
- [SSH Keys](#ssh-keys)
- [Logging-In](#logging-in)
- [Uploading](#uploading)
- [Downloading](#downloading)
- [How To Find Out What Branch Your Editing](#how-to-find-out-what-branch-your-editing)
- [Creating A Branch](#creating-a-branch)
- [Merging](#merging)
- [Making A Repo](#making-a-repo)
- [References](#references)


----------


# Installing Git Software

 - `sudo apt-get install git` **# for Debian/Ubuntu users**
 - `brew install git` **# for Mac OS X users with Homebrew installed**
 - https://git-scm.com/ **# Windows**
 


----------


## SSH Keys

 - `ssh-keygen -t rsa -C "your_email@example.com"`
 - Then Upload Your Public Key <a href="https://github.com/settings/ssh ">Here</a>


----------

## Logging-In

 - `git config --global user.email "you@example.com"`
 - `git config --global user.name "Your Name"`


----------

## Uploading

 - `git add <file>` or `git add *`
 > Use the second one if you need to upload all changed files
 - `git add -u`
 > Tells git to acknowledge deleted files
 - `git commit -m "comment"`
 - `git push`  **#Current Branch**
 - `git push origin <branch>` **#Other Branch**
 


----------

## Downloading

 - `git clone <repo> ` **#First Time**
 - `git pull ` **When In The Local Repo Folder & After The First Time**
 - 
----------
## How To Find Out What Branch Your Editing:
 - `git status`


----------

## Creating A Branch

 - `git checkout -b <new-branch> <existing-branch>` **# -b Tells Git You Want To Make A New Branch**
 - `git checkout <branch> `  **#Switch Between Branches**
 - `git stash` **#Use If Your Branch Still Needs Some Work And You Need To Switch Branches**
 


----------
## Merging

 - `git checkout master ` **#Resolve Any Merge Conflicts If There Are Any**
 - `git merge development `  **#Git Merge Development**
 - `git merge master` **on branch development**


----------
## Making A Repo

 - `git init`
 - `git add`
 - `git commit -m "comment"`
 - Login To GitHub
 - Click the new repository button in the top-right. You’ll have an option there to initialize the repository with a README file, but I don’t.
 - Click the “Create repository” button
 - `git remote add origin git@github.com:username/new_repo` or `git remote add origin https://github.com/username/new_repo`
 - `git push -u origin master`


----------

## References

 - https://help.github.com/articles/adding-a-file-to-a-repository-using-the-command-line/
 - https://dont-be-afraid-to-commit.readthedocs.io/en/latest/git/commandlinegit.html      
 - https://confluence.atlassian.com/bitbucketserver/creating-ssh-keys-776639788.html      
 - https://github.com/settings/ssh 
 - http://kbroman.org/github_tutorial/pages/init.html				       
 - https://stackoverflow.com/questions/3055492/git-best-practices-for-quickly-switching-between-branches
 - https://stackoverflow.com/questions/14168677/merge-development-branch-with-master
 - https://gnupg.org/download/index.html
 - https://ssd.eff.org/en/module/how-use-pgp-windows	
 - https://help.github.com/articles/signing-commits-using-gpg/
