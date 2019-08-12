# Table of contents
- [Install on windows](#install-on-windows)
- [Creating your first git repository](#creating-your-first-git-repository)
  - [Create a git folder for your repositories](#create-a-git-folder-for-your-repositories)
  - [Create a local repository](#create-a-local-repository)
  - [Add your first file](#add-your-first-file)
- [How to get Started with GitHub](#how-to-get-started-with-github)
  - [Create a GitHub account](#create-a-github-acccount)
  - [Generating SSH key](#generating-an-ssh-key)
  - [Push local repo to GitHub](#pushing-local-repo)
- [Group assignment](#group-assignment)
- [Resources](#resources)

## Install on Windows
1) Download git from [here](https://git-scm.com/downloads)
2) Go through the installer steps. It is recommended to look at every step, but if you do not understand a 100%, the default settings are OK

3) ...
4) Profit! You have installed git

> __NOTE__: The following parts all use the commandline. Windows users are recommended to install a decent terminal. If you do not have one, the Git Bash terminal will work as well 

## Creating your first git repository
It is good practice to have your git repositories in one place.
For the following paragraphs, our git folder will be in `C:\Users\user\Documents\`

### Create a git folder for your repositories
Open up the terminal and enter the following commands

```bash
cd ~\Documents
mkdir git
cd git
```
This folder can be used to store all your git repositories

### Create a local repository
Next we'll create a seperate directory which is going to become our first git repo

```bash
mkdir hello_git
cd hello_git
git init
```

### Add your first file
Create a python file by entering the following command

```touch hello.py```

Open edit mode by entering ```vim hello.py```, if you prefer nano that's fine, I've chosen vim as it comes preinstalled on most OS   
Press ```i``` to enter insert-mode and insert some text in the file by typing ```print('Hello GitHub!')```  
Press ```Esc``` to exit insert-mode, save and close the file by entering ```:wq```


Great! Now let's add and commit your file to your local repository

```bash
git add .
git commit -m "initial commit"
```

Your files and changes are now saved in your local repository, next we'll 
work on pushing the files to GitHub so your code is always backed-up and 
shareable with people around the world.

## How to get started with GitHub

### Create a GitHub account
Go [here](https://github.com/join) and create an account. Make sure to select the Free subscription.

### Generating an SSH key
SSH keys are used for authentication and allow you to connect to GitHub without supplying your username and password every time.
Read on how to create your SSH key [here](https://help.github.com/en/enterprise/2.15/user/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

### Push your local repo to GitHub
First, go to Github and in the topright click 'New repository'
Name the repository "hello_git", leave all the other settings as they are and click 'create'  
At the top of the hello_git repo you'll find a quick setup. Copy either the link for HTTPS or SSH  
Enter the following commands in GitBash:

```bash
git remote add origin <paste url here>
git push origin master
```

You've done it! Your first piece of code is now pushed to GitHub.

## Group assignment
If you're in an instructor led class you can now go to the folder group_assignment and follow the instructions

## Resources
