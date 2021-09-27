

# Git Tutorial

Pada tutorial kali ini kita akan membahas mengenai git dan everything about git (dasar only bruh)

---

# Table of Contents
* [Git Init](#Git-Init)
* [Git Clone](#Git-Clone)
* [Git Add](#Git-Add)
* [Git Commit](#Git-Commit)
* [Git Pull](#Git-Pull)
* [Git Push](#Git-Push)
* [Git Status](#Git-Status)
* [Git Log](#Git-Log)
* [Git Branch](#Git-Branch)
* [Git Checkout](#Git-Checkout)
* [Git Merge](#Git-Merge)

---

## Git Init
This command creates an empty Git repository - basically a .git directory with subdirectories for objects, refs/heads, refs/tags, and template files. An initial branch without any commits will be created.  

To create new repository on a folder use

```
git init
```

Don't forget to check the folder. It should have hidden .git folder and it means you have successfully create local repository 

## Git Clone
This command is for downloading existing source code from a remote repository (i.e Github). In other words, Git clone basically makes an identical copy of the latest version of a project in a repository and saves it to your computer. This will make a copy of the project to your local workspace so you can start working with it.  

To clone repo from github to local we use
```
git clone <repo-link>
```
after we use this it should have a new folder named exactly like in the github. We also can  specify the name of the folder by using
```
git clone <repo-link> <name>
```
Example
```
git clone https://github.com/gdscitb/HandsOn-2021.git gggaming
```
## Git Add
This command will move our file to staged changes.  

To add all the files to the staged changes use
```
git add .
```
You can also add one or more file by specify the name of the file
```
git add <filename>
```

Example
```
git add file1.txt file2.txt
```

## Git Commit
This command is like setting a checkpoint in the development process which you can go back to later if needed. It creates a new commit containing the current contents of the index and the given log message describing the changes.

To commit our changes use
```
git commit -m <commit-message>
```
Example
```
git commit -m "adding file1.txt, updates file2.txt..."
```
Commit message should be meaningful.
## Git Status
This  command displays paths that have differences between the index file and the current HEAD commit, paths that have differences between the working tree and the index file, and paths in the working tree that are not tracked by Git.

To use it type
```
git status
```
It will display in what branch you are working, status different between local and remote repository
## Git Log
To show the commit log use 
```
git log
```
it will list all of the commits that you have done
## Git Branch
Git branch can list, create or delete branch in repo.  
To list all the branch use
```
git branch --list
```
To create new branch use
```
git branch <nama-branch>
```
To delete branch use
```
git branch -d <nama-branch>
```

## Git Checkout
This command can update our file before or after commit. In short, it can traverse through list of commit tree or change to another branch.  

We can move to another commit by using
```
git log
git checkout <nama-commit>
```
We can also move to another branch by using
```
git checkout <nama-branch>
```
## Git Pull
This command will update our local repo to the newest commit on the remote repo

```
git pull
```
## Git Push
This command will update the remote repo to newest commit, while sending the update from local to repo.

```
git push
```
## Git Merge
This command will merge changes from one branch into another (normally it would be main)

```
git merge <nama-branch>
```
Example
```
git merge branch2
```

---

Note: **Make sure that you are in the right directory before use all the commands, otherwise it wont work**

# Reference Material
* [Git Documentation](https://git-scm.com/book/en/v2)
* [Missing CS MIT EDU](https://missing.csail.mit.edu/2020/version-control/)
* [Panduan Ringkas](https://rogerdudler.github.io/git-guide/index.id.html)  


