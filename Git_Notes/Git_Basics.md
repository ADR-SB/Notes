# Git Basics

###  What is Git?

Git is a distributed version control system (VCS) or source control system. A VCS is an application that keeps track of your code and all the changes that are made to it. It also allows us to share our code with others and collaborate with one another without overwriting each other’s changes. In this course, we are going to give you a brief overview of Git and teach you how to save your code to a repository.

---
### Why Source Control?

Source control management systems are designed to keep history and revision information about the files and projects stored within a repository. By storing this information, we have a complete history of everything that happened to the projects within the repository. In the event of a catastrophe, we can recover a previously saved version. Also, by saving our changes, we can easily share work with other developers and collaborate on projects regardless of location.

---
### Git's Origins

Git was created by Linus Torvalds, who is known as the father of Linux. Torvalds became frustrated with the processes used by the Linux development community and wanted to create a better way to share code with other open-source developers who were working on the platform. Git came into being in 2005 with five primary goals: speed, simple design, support for parallel branches and fully distributed workflows, and the ability to handle large projects.

---
### Why Choose Git?

There are many reasons for choosing Git.
- Git is cross-platform: it works on Windows, Mac, and Linux.
- Git is an open-source project and does not have any licensing costs. You may need licensing if you choose to use an established online provider or if you choose to purchase third-party tools, but the system itself does not have licensing costs.
- Git is also easy to learn and can be very simple, but it offers complex features that you can take advantage of if you need them or as you grow and require more of their use.

---
# Basic Git Commands

## Add, Commit, Pull, Push

### Add

To add a file to the repository, we can use the add command. Open your Git command tool (Git Bash or Terminal for example) and use the cd command to navigate to your local repository.
$ cd '[path to directory]'
Once you are there, you can run the following command:
```
$ git add --all
```
The use of the --all parameter ensures that all files in all subdirectories will be staged, including new files, modified files, and any files removed from the repository. Alternatively, you can name specific files, which can streamline things if the repo is large and you have only changed a few files.
It is important to note that even though a file may physically exist in the directory, it will not be tracked by Git and included in your repository until it is "added" to the repository using the add command, so you should always run git add before running git commit.

---
### Commit

The git commit command will create a new save point in the history of the repository. These are the points we review and care about when it comes to the repository. They provide the save points in the repository that allow us to return to the exact state of the files as they existed at that moment we did the commit.
```
$ git commit -m "[MESSAGE]"
```
Replace [MESSAGE] in the command above with your description for this save point in the repository. This should be a relatively short message that explains why you are committing this code or what state the code is in at that point in time. For example, if you have just added a Contact page to a website, an appropriate commit command might look like this:
```
$ git commit -m "new contact page in website"
```
Whether you are describing a new feature you added or a bug that you fixed, this information will help you and your collaborators understand the purpose of the changes.
The Commit Message is Required

Each time you commit changes, you must include a message that describes changes made since the last commit. If you forget to include the -m option with the message, the command line window will open a text editor for that message. When this editor opens, it displays an empty window with the cursor at the top of the window. This is a Linux-based editor that can be difficult to navigate. By default, the content is read-only, so to enter the message, you may have to hit the "i" key to begin inserting characters. When you have finished making changes, hit the Esc key and then Shift + : (colon) to move the insertion point to the command line at the bottom of the editor window. Enter the command wq to write the file and quit. This can be an unpleasant experience if you are not familiar with these tools, so it is best practice to include the -m modifier and a message when performing a commit from the command line.

---
### Pull

We pull from the remote when we have or someone else has checked code into it from another computer and we need to get those changes on our local machine. Pulling changes from a remote repository is quite easy. We run the git pull command.
```
$ git pull [repository] [branch]
```
The git pull command allows us to specify the remote repository and the branch within that repository, which is useful if we are working in multiple repositories. If you are working in the original repository, then the easiest way to reference it is with the parameter origin.
Branches are a little more complicated. By default, the initial branch of any repository is called main, and as a starting point, you will use the command:
```
$ git pull origin main
```
You can leave off the repository and branch information, but it's a good habit to always include them to be sure you are getting the files you expect to get.

---
### Push

The git add and git commit commands only make changes within your local Git installation, and they will not change any files stored in the online repository. To send the committed files to the repository, you must use git push, whose syntax is similar to git pull:
```
$ git push [repository] [branch]
```
To push files to the main branch of your original repository, the command is:
```
$ git push origin main
```
After pushing changes, you should see the changes in your GitHub repository and those changes will be visible to your instructor.

---
### Branching

As you work on a project (or especially if you are working on a project in a team of developers), though, you may want to create a new branch to work on so that your changes don't affect the main branch that other people may be working in. Essentially, a branch is a copy of a repository with its own name but that Git still associates with the initial main repository. After you have made changes to the code in your own branch, you can easily merge those changes to the main branch and make them available to everyone else on the team.
Using a new branch involves two steps: create a branch and check it out in Git. The commands look like this:
```
$ git branch [branch-name]
$ git checkout [branch-name]
```
As a rule of thumb, while it is possible to use git push without specifying a repository and branch, you should always name them to be sure you know where those files will show up in GitHub.

#### ⚠️ Important ⚠️ 
The git checkout command changes your local Git installation to use that branch by default for all future pushes. If you use branches, it is important to always name the branch you want to use in any git push command.
If you want to check to see what branch is currently active in Git, use the git status command.

---
## Summary

It is a good idea to get in the habit of always pulling your repository after you have done a commit but before you do a push. This pattern of add, commit, pull, push will allow you to do the following:
1. Add: Start tracking new files and changes when you finish the code you are working on.
2. Commit: Create a save point for your changes in the repository.
3. Pull: Retrieve other code changes from the remote repository AND merge those changes with your own. This is important because if there are any conflicts between the code you have written and committed and the code that you have pulled from the remote repository, you will need to fix it before you send it to the remote server.
4. Push: Send the committed code to the remote server.
Git has far more commands than the ones we covered here. It is a complex system with many options for tracking our code changes over time and allowing collaborative work on application source code. However, using a simple workflow like the one we described here works well for most small teams and projects.

---
