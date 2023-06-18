---
# Common-Defined params
title: "How to Start Using Git"
date: "2023-06-15"
description: "Hot to Git"
categories:
  - "How To"
tags:
  - "how-to"
  - "git"
  - "coding"
menu: main # Optional, add page to a menu. Options: main, side, footer

# Theme-Defined params
thumbnail: # Thumbnail image
lead: "Learn the basics of Git" # Lead text
comments: false # Enable Disqus comments for specific page
authorbox: true # Enable authorbox for specific page
pager: true # Enable pager navigation (prev/next) for specific page
toc: true # Enable Table of Contents for specific page
mathjax: true # Enable MathJax for specific page
sidebar: "right" # Enable sidebar (on the right side) per page
widgets: # Enable sidebar widgets in given order per page
  - "search"
  - "recent"
  - "taglist"
---

We are going to create a repository and push some code to it. Then we are going to explore how to further manage the repo.
<!--more-->



## Getting Started
---
<br>

We are going to create a repository and push some code to it. Then we are going to explore how to further manage the repo.

<br>

Here is the order of operations we will be following:

<br>

1. Make directory
2. Git Init
3. Add Remote Repo
4. Set Upstream Branch
5. Create File(s)
6. Check File(s)
7. Check Status
8. Commit
9. Check Log
10. Push
11. Checkout Previous Commit
12. Checkout Back to Master
13. Pull
14. Clone

<br>

To do this, we will need the following:


- Windows Powershell
- Git
- Github Account

<br>



### Make Directory & Initialize Git
---
<br>

We need to make a folder to act as the local directory for our repository. To do this, launch powershell and navigate to where you want the directory located. We can use the *mkdir* function which calls the *New-Item* cmdlet to create a directory for us. We will than want to use *cd*, which is an alias for the *Set-Location* cmdlet, to switch to the folder we've created. We can then call the git executable and feed it a command to initialize our repo. Like this:

```shell
mkdir your_folder_name_here
cd your_folder_name_here
git init
```

<br>
<br>
<br>

### Add a Remote Repository and Set Upstream Branch
---

<br>

In order to be able to push and pull from our repo on Github as well, we need to set a remote repository to use. We can do this by calling git and using the *remote add* command to assign a URL to a name. 



```shell
git remote add <name> <url>
```
<br>

Its standard to name the main remote repo **Origin**, and then the URL would be your repository in Github. Here is a real life example:


```shell
git remote add Origin https://github.com/impliedbelligerence/hackypi-tests
```

<br>

If we need to change our remote repository later, we can do so like this:

```powershell
git remote set-url <name> <new url>
```

<br>

And if we need to see what the current remote repo is set to, we can do this:
```powershell
 git remote get-url --all <name>
 ```

 <br>

We then will need to a branch to act as the "upstream branch", which is basically the branch everything will get published to. We do this by calling git and using the push command with a parameter to set the upstream branch. 

```powershell
git push --set-upstream <name> <branch>
```

<br>

And a real life example:


```powershell
git push --set-upstream origin master
```
<br>
<br>

### Make Files, Add Files, Check Status & Commit
---

<br>

Before we can add anything to our repo on Github, we will need to make some files, add them to be commited and then commit them to our local repository first. We should do a check or two along the way as well.  

Create a random file of any type and place it into the directory using the *New-Item* cmdlet. We can then check the status of our local repo to see what changes have been made by calling *git* and using the command *status*.. We will use this information to stage specific files we want commited to our local repo using git's *add* command. Once we have some files staged, we can go ahead and commit the changes to our local repro using git's *commit* command. We can use the -m parameter to leave a message with our commit

<br>

```powershell
New-Item test.txt
git status
git add test.txt
git commit -m "Init Commit"
```

<br>

If we just need to add all changes to be staged, we can do that like this:
```shell
git add .
```
<br>

And if we check the commit log, we can do this:
```shell
git log
```

<br>
<br>

### Checkout A Commit and Then Switch Back to Master Branch
---

<br>

After we make a new commit to our local repo, we can check the log for the hash of any previous commits and check them back out to poke around. First we will need to make a second commit to our local repo.

```shell
git log
git checkout <commit hash>
```

<br>

Now our local repo has been switched to a previous version and any additional commits we make will go to this branch. If we want to go back to our master branch, we can do this:

```shell
git checkout Master
```

<br>

If we need to see the branches in the repo, we can do this:

```shell
git branch
```

<br>
<br>


### Push to Remote Repository
---

<br>

Once we have the changes to our local repo commited, we can go ahead and push the changes to a branch in our remote repo. We can do this by calling *Git* and using the *push* command, we can also specify a branch to push to if we need to push if there are multiple branches in the repo.

```powershell
git push master
```

<br>




git config -l

.\filename.py - launch file 