# Git + Github Intro

## What is Git?
`Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.` Definition by [Git Official Site]('https://git-scm.com/')
## OK, so what is Git?
  Imagine you are a coder who finds a parallel universe jumping and time traveling machine that only works for your code. Your machine would be Git. 
## What do I use this powerful machine for?
  You are working, you have a deadline tomorrow. If you work on the same code without using your Git machine you are probably going to make mistakes, delete files accidentally, get confused and work on something for an hour just to realize that the initial code was better, etc. You might also break your website in the process of adding a new feature... Or maybe you want to take a break from the about us page and work on the contact form for a while, then come back to it later. Git gives you the possibility to work clean, to be able to go back to changes you made in the past or to jump into another feature without finishing the original one, and much more.
## But what is GitHub/GitLab/etc? 
  GitHub/GitLab/etc is your Git in the cloud. All the work you do with the Git machine, you can upload it to a new 'repository' (project!) to access it later, to share with other people and work collaboratively.

##Let's go!

## Common terminal commands
These commands work in any terminal, they are independent from Git.
- `cd` navigates to a folder. I.e.: `cd b:/dev/newrepo`
- `mkdir`makes a new directory (folder). I.e.: `mkdir newfolder` 
- `ls` shows you the content of the folder you are in.
- `rm` deletes a file or folder. I.e.: `rm newfolder`

## Common Git terms
- Working directory: the folder where we are currently working.
- Staging area (git index): contains all the changes that are ready to be committed and that you have added with `git add`. To 'stage' a file means to put that file to the side, to be committed later.
- Local Repository (.git): your git initiated 'project' in your computer
- Remote: whatever is not in your local machine but on the internet. 
- Branch: it's a deviation of your original code. You have a starting point in your code (master or main branch), you branch it and you continue working on it. You will have the "base" of where you started but at the same time new code that is not on your main branch. When you are done coding on your new branch, you can "merge" it with your starting point (main branch). You can have as many branches as you want.
 
## Common Git Commands
- `git init` starts a new local repository
- `git status` shows you the files that have been modified but not committed 
- `git add` adds the files that have been edited so you can track changes
  - `git add .` adds all the files that have been edited
   - `git add src/` adds all the content that has been edited in the folder of your choice
- `git rm` removes files that has been staged
- `git commit`
   - `git commit -m 'this is a new commit'` commits all the files added previously with `git add`
- `git checkout` takes you to another branch
  - `git -b 'new-branch-name'` creates a new branch and takes you there
- `git log` shows you a list of commits on the branch
- `git push` 'uploads' your last commits to the branch
- `git pull` 'downloads' whatever content you have on the same branch in the remote origin
  - `git pull origin master` 'syncs' your branch to the content in master
- `git reset` resets all the files in your current branch
  - `git reset --hard origin/master` resets all your files to the branch of your choice. I.e.: `git reset --hard origin/newrepo`
- `git reset --hard HEAD` HEAD is a keyword used to move around commits in your branch. If you run this command, your files will be reseted to the indicated commit. 
  - Going back two commits instead of one: ``git reset --hard HEAD~1`
 
## Initializing a new repository
- Create and navigate to a new folder
- `git init` to create a new repository in your local machine

## Linking your git repository with your Github account
- Go to your Github account and create a new repository
- Go back to your console, cd into your active project and type:
- `git remote add origin https://github.com/your_username/your_repository_name.git`
- Now everytime you push a commit it will be uploaded to your github repository

 
