# Basic Git Commands

#### Username & Email Setup:

Username: 
```
git config --global user.name "username"
```

Email: 
```
git config --global user.email email@domain.com
```

Example:
```
git config --global user.name "Caitlin Stuart"
git config --global user.email "cstuart@email.com"
```
---
#### Creating new directory (Folder):
```
mkdir DirectoryName
```

Example:
```
mkdir Git_folder
```
---
#### Creating new File:	
```
touch Filename
```

Example:
```
touch fileA
```
---
#### add:
Adds files to the staging area.
* add --all : Adds all changes throughout the entire repository, including new, modified, and deleted files, and stages them for commit.
```
git add –all
```
* add * : Adds all changes in the current directory, but doesn't include changes in subdirectories or untracked files.
```
git add *
```
* add . : Adds all changes in the current directory and its subdirectories, but doesn't include changes to untracked files.
```
git add .
```
* To add a specific file
```
git add filename
```
(Always add before commit)

---
#### commit:	
```
git commit -m "[MESSAGE]"
```

Example:
```
git commit -m "new contact page in website"
(must include a message that describes changes made since the last commit)
```
---
#### push:
```
git push [repository] [branch]
```

Example:
```
git push origin main
```
---
#### pull:	
```
git pull [repository] [branch]
```

---
#### Branch:	
```
git branch branchname
```
(Creates a new branch but will not checkout to it. You have to checkout or switch to that branch)

---
#### Checkout:	
* Checkout from the current branch to the branch specified.
```
git checkout branchname
```
* Creates a new branch and checkouts to it. 		  
```
git checkout -b branchname
```		  
* create a new local branch named branchname that tracks the origin/branchname remote branch.Usually done after cloaning an existing repo, ie when an existing repo with multiple branches are cloned there will not be any local branch that will keeps track of the changes happining to the remote , so when we check out of the main branch we will create a new local branch that tracks the remote branch
```
git checkout -b branchname origin/branchname
```
		
---
#### Switch:	
```
git switch branchname
git switch -c branchname
```
		
---
#### Delete branch:	
```
git branch -d branchname
```
---
#### Delete file:	
```
git rm filename
```
(If the file has already been committed, you'll also need to commit the deletion: `git commit -m "Deleted filename"`)

---
#### Delete directories:	
```
git rm directoryname
```
(Only works if directory is empty. After running this command, you'll need to commit the deletion: `git commit -m "Deleted directoryname"`)

* If the directory contains files or other directories, you'll need to use the -r flag to recursively remove its contents.
```
git rm -r directoryname
```
		
---
#### List all branches:	
```
git branch
```
```
git branch -a
```
---
#### List all remote repos:	
```
git remote -v
```
---
#### Merge:	
```
git merge <branch_name>
```
(Go to the source branch with checkout then specify the target branch in branch_name) 

---
#### Status: 	
It shows information about files that have been modified, staged, or untracked.
```
git status
```
Example:
```
$ git status
On branch newbranch
nothing to commit, working tree clean
```
---
#### Path:	
`Pwd`

---
#### Navigation:	
`cd <path>`

---
#### History:	
Shows all the previously executed commands.
```
history
```
		
---
#### Log:	
```
git log
git log --oneline
git log --graph
git log --author=<author>
git log --since=<date>
```
---
#### setting upstream tracking branch:
Setting the upstream branch for the local branch newbranch to the remote branch origin/newbranch.
```
git branch --set-upstream-to=origin/newbranch newbranch
```
---

