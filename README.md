# githubtraining
## What is Git?
`Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.` Definition by [Git Official Site]('https://git-scm.com/')
## OK, so what is Git?
  Imagine you are a coder who finds a parallel universe jumping and time traveling machine that only works for your code. Your machine would be Git. 
## What do I use this powerful machine for?
  You are working, you have a deadline tomorrow. You have many features to develop, you have to create homepage, an about us page and a page with a contact form. If you work on the same code without using your Git machine you are probably going to make mistakes, delete files accidentally, get confused and work on something for an hour just to realize that the initial code was better, etc. You might also break your website in the process of adding a new feature. Maybe you want to take a break from the about us page and work on the contact form for a while, then come back to it later. Git gives you all these possibilities and more. 
## But what is GitHub/GitLab/etc? 
  GitHub/GitLab/etc is your Git in the cloud. All the work you do with the Git machine, you can upload it to a new 'repository' (project!) to access it later, to share with other people and work collaboratively.
  

## Common terminal commands
These commands works in any terminal, they are independent from Git.
- `cd` navigates to a folder. I.e.: `cd b:/dev/newrepo`
- `mkdir`makes a new directory (folder). I.e.: `mkdir newfolder` 
- `ls` shows you the content of the folder you are in.
- `rm` deletes a file or folder. I.e.: `rm newfolder`

## Common Git terms
- Working directory: the folder where we are currently working.
- Staging area (git index): contains all the changes that are ready to be committed and that you have added with `git add`. To 'stage' a file means to add it so you can commit it.
- Local Repository (.git): your git initiated 'project' 
- Branch: you take a picture
 
## Common Git Commands
- `git init` starts a new local repository
- `git status` shows you the files that have been modified but not committed 
- `git add` adds the files that have been edited
  - `git add .` adds all the files that have been edited
   - `git add src/` adds all the content that has been edited in the folder of your choice
- `git rm` removes files that has been staged
- `git commit`
   - `git commit -m 'this is a new commit'` commits all the files added previously with `git add`
- `git checkout` takes you to another branch
  - `git -b 'new-branch' creates a new branch and takes you there
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
- `git init` to create a new repository
