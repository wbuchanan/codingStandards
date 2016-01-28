---
layout: page
title: Version Control 
permalink: /version-control/
---

# Intro to Git and Version Control Systems

## What are version control systems?

## What is Git?

## Why use Git?

## Where do you get Git?
The first step is to get the software on your workstation.  You can download the Git binary from [http://www.git-scm.com](http://www.git-scm.com).  If you are using a Mac/OSX open the Terminal application (/Applications/utilities/Terminal.app) then copy and paste the following into the terminal:

``` 
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Chances are you will also need to install the Apple application [Xcode](https://developer.apple.com/xcode/download/) for some of the tools you may want to install later (the Xcode application provides a few different compilers and command line utilities for OSX).  If using a Debian based *nix you can `sudo apt-get install git` and if you are using a RedHat derivative you can use `sudo yum install git` to accomplish the same.  

If you are not using a *nix-based platform, you will want to make sure to install Git Bash (it is an option when you download Git from the link above).

## Create a repository - git init


## Make sure not to store sensitive data in your repository - The .gitignore file
Since the majority of our data is protected under FERPA, you should make sure that you do not store any copies of sensitive data in your repository.  The easiest way to do this is by creating a .gitignore file.  If you are in the Git Bash application - or a terminal - you can do this by modifying the code below to point to the directory where your repository exists:

```
# First change directories to the location of your repository
cd ~/myGitRepo

# Now you can open the vi editor to create the .gitignore file
vi .gitignore

# Once the vi editor starts up, press the letter `a` on your keyboard to enter into insert mode
# Then add the following lines to the file
*.csv
*.xlsx
*.txt
*.dta
*.sav
*.por
*.sas7bdat
*.RData
*.Rdata
*.Rds
*.dat

# After adding those lines press the `esc` key then enter `:wq` to save the file and close vi
# Now if you run the command:
git status

# You should see the new .gitignore file, and should see that none of the files with the types listed above are being tracked
```

## Save your changes - git add && git commit 


## Create a new version of your project - git branch


## Get a copy of existing code for your use - git clone 


## Add a remote repository to store a copy of your code - git remote add


## Update your changes on GitHub/Gitlab - git push 


## Submit changes/updates to collaborative projects - git pull



