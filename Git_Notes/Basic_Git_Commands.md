# Basic Git Commands
------------------------------------------------------------------------------------------------------------------------------------------
#### Username & Email Setup:	
	Commands:
		- Username: git config --global user.name "username"
		- Email: git config --global user.email email@domain.com

	Example:
		git config --global user.name "Caitlin Stuart"
		git config --global user.email "cstuart@email.com"
------------------------------------------------------------------------------------------------------------------------------------------
#### New Directory (Folder):	
	Command:
		- mkdir DirectoryName

	Example:
		mkdir Git_folder
------------------------------------------------------------------------------------------------------------------------------------------
#### New File:	
	Command:
		- touch Filename

	Example:
		touch fileA
------------------------------------------------------------------------------------------------------------------------------------------
#### add:	
	Command:
		- git add –all
		- git add .
		- git add filename
		  (Always add before commit)
------------------------------------------------------------------------------------------------------------------------------------------
#### commit:	
	Command:
		- git commit -m "[MESSAGE]"

	Example:
		git commit -m "new contact page in website"
		(must include a message that describes changes made since the last commit)
------------------------------------------------------------------------------------------------------------------------------------------
#### push:	
	Command:
		- git push [repository] [branch]

	Example:
		git push origin main
------------------------------------------------------------------------------------------------------------------------------------------
#### pull:	
	Command:
		- git pull [repository] [branch]

------------------------------------------------------------------------------------------------------------------------------------------
#### Branch:	
	Command:
		- git branch branchname
		  (Creates a new branch but will not checkout to it. You have to manually go to that branch)
------------------------------------------------------------------------------------------------------------------------------------------
#### Checkout:	
	Command:
		- git checkout branchname
		  (Checkouts from the current branch to the branch specified)

		- git checkout -b branchname
		  (Creates a new branch and checkouts to it) 

		- git checkout -b branchname origin/branchname
		  (This will create a new local branch named branchname that tracks the origin/branchname remote branch.
		  Usually done after cloaning an existing repo, ie when an existing repo with multiple branches are cloned there will not
		  be any local branch that will keeps track of the changes happining to the remote , so when we check out of the main 
    		  branch we will create a new local branch that tracks the remote branch)
------------------------------------------------------------------------------------------------------------------------------------------
#### Switch:	
	Command:
		- git switch branchname
		  (Switches from the current branch to the branch specified)

		- git switch -c branchname
		  (Creates a new branch and checkouts to it) 
------------------------------------------------------------------------------------------------------------------------------------------
#### Delete branch:	
	Command:
		- git branch -d branchname
------------------------------------------------------------------------------------------------------------------------------------------
#### Delete file:	
	Command:
		- git rm filename
		  (If the file has already been committed, you'll also need to commit the deletion:
		  git commit -m "Deleted filename")
------------------------------------------------------------------------------------------------------------------------------------------
#### Delete directories:	
	Command:
		- git rm directoryname
		  (Only works if directory is empty. After running this command, you'll need to commit the deletion:
		  git commit -m "Deleted directoryname")


		- git rm -r directoryname
		  (If the directory contains files or other directories, you'll need to use the -r flag to recursively remove its contents)
------------------------------------------------------------------------------------------------------------------------------------------
#### List all branches:	
	Command:
		- git branch
		- git branch -a
------------------------------------------------------------------------------------------------------------------------------------------
#### List all remote repos:	
	Command:
		- git remote -v
------------------------------------------------------------------------------------------------------------------------------------------
#### Merge:	
	Command:
		- git merge <branch_name>
		  (Go to the source branch with checkout then specify the target branch in branch_name)
------------------------------------------------------------------------------------------------------------------------------------------
#### Status: 	
	Command:
		- git status
		  (It shows information about files that have been modified, staged, or untracked.)

	Example:
		$ git status
		On branch newbranch
		nothing to commit, working tree clean
------------------------------------------------------------------------------------------------------------------------------------------
#### Path:	
	Command:
		Pwd
------------------------------------------------------------------------------------------------------------------------------------------
#### Traversing:	
	Command:
		cd <path>
------------------------------------------------------------------------------------------------------------------------------------------
#### History:	
	Command:
		history
		(Shows all the previously executed commands)
------------------------------------------------------------------------------------------------------------------------------------------
#### Log:	
	Command:
		- git log
		- git log --oneline: Displays each commit on a single line, showing only the abbreviated commit hash and the commit message.
		- git log --graph: Displays the commit history as a text-based graph, showing the relationships between commits and branches.
		- git log --author=<author>: Filters the commit history to only show commits by a specific author.
		- git log --since=<date>: Filters the commit history to only show commits since a specific date.
------------------------------------------------------------------------------------------------------------------------------------------
#### setting upstream tracking branch:
	Command:
		git branch --set-upstream-to=origin/newbranch newbranch
		(Setting the upstream branch for the local branch newbranch to the remote branch origin/newbranch.)
------------------------------------------------------------------------------------------------------------------------------------------

