![Git & Github] (img/)

# Git and Github Basics

Taking you from the very basics of Git, version control, and Github to the most common
processes you will use.

## Table of Contents
- [What is Git](#what-is-git)
- [What does Git do](#what-does-git-do)
- [Getting Started with Git](#getting-started)
- [Working with Github](#working-with-github)

## What is Git

-   Git is a free open source version control system.
-   Git is used to:
    -   Track code changes
    -   Track who made changes
    -   Collaborate during coding

### What does Git do

-   Manage projects with **Repositories**
-   **Clone** a project to work on a local copy
-   Control and track changes with **Staging** and **Committing**
-   **Branch** and **Merge** to allow for work on different parts and versions
    of a project
-   **Pull** the latest version of the project to a local copy
-   **Push** local updates to the main project

### Getting Started
1. #### Download Git from [git-scm](https://git-scm.com/)
2. #### Using Git on the Command line ->
    - open your terminal
    - Windows can use GitBash, installed with Git
3. #### Check your version of Git

```bash
git --version
# or
git -v
```
4.  #### Let git know who you are

- Create an account on [Github](https://github.com)
- In terminal, configure your name and email.  So Git knows who is making the changes
- Use global to ser the username and email for every repository on your computer
- If you want to set the username/email for just the current repo, you can remove ```
--global ```

```bash
git config --global user.name "John Doe"
git config --global user.email "JohnDoe@example.com"
```

5. ### Create a project to work in
- If you already have a folder that you use, then navigate to it using the terminal

```bash
#make a new directory
mkdir your_folder_name
#change to the current working directory
cd your_folder_name
```

6.  Initialize Git
```bash
git init
```

- Git knows that it should watch the folder that you initialized it on
- Git creates a hidden folder to keep track of the changes

```
# how to show the folder in VS Code
Code|File -> preferencs -> settings
Search for "exclude" to find the default exclude list
Edit ".git" extension to remove t from the list and allow it to be visible in VS Code
```

7. ### Open in text editor and add some files
- There is a shortcut to open current working directory in VS Code. 
```bash
# open in VS Code
code .
# create a file
touch file_name
```

8. ### Let's work with files
```bash
# create a new file
touch index.html
```
9. #### Check the status of the repo
```bash
git status

# check with the compact output

git status --short

# Short status flags are:
    # ?? - Untracked
    # A - Files are added to stage
    # M - Modified
    # D - Deleted files
```
- Git is aware of the file but     

10. Staging our files
```bash
# add our file to the staging environment

git add index.html

# or add multiple files at once

git add --all

# or 

git add .
```

11. #### Committing our Files
- moving from staging to commit
- Adding commits keeps track of our process and changes
-Git considers each commit as a snapshot of our project at the time 
of the commit.  We can use these snapshots to revert to earlier versions.

```bash
# The commit command performs a commit and the -m "message" adds a message.

git commit -m "your message"
```

12. #### Commit Log

```bash

git log
```

13. #### Git Help

```bash

git help --all

# allows us to see all the possible git commands
```
### 15.  Working with Github

1. Create | Log into Github
2. Create an empty repo onGithub
3. Push our local repo to Github



