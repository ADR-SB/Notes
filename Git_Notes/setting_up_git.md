# Setting Up Git
--------------------------------------------------------------------------------------------------------------------------------------------------------------------
### Here are the typical steps for installing Git on various operating systems:
--------------------------------------------------------------------------------------------------------------------------------------------------------------------
### For Windows:
1. Download the Git installer from the official Git website ([https://git-scm.com/](https://git-scm.com/download/win)).
2. Run the installer executable file (.exe).
3. Follow the installation wizard's instructions, selecting the desired components and installation directory.
4. Choose the default options for most settings unless you have specific preferences.
5. Complete the installation process.
6. Open a new command prompt or Git Bash terminal to verify the installation by typing `git --version`.
--------------------------------------------------------------------------------------------------------------------------------------------------------------------
### For macOS:
1. Git comes pre-installed on macOS, but you can update it if needed. Open the Terminal app.
2. Install Homebrew if you haven't already (https://brew.sh/).
3. Run `brew install git` in the Terminal to install Git using Homebrew.
4. After the installation is complete, verify it by typing `git --version`.
--------------------------------------------------------------------------------------------------------------------------------------------------------------------
### For Linux (Ubuntu/Debian):
1. Open the terminal.
2. Update the package index: `sudo apt update`.
3. Install Git: `sudo apt install git`.
4. After the installation is complete, verify it by typing `git --version`.
--------------------------------------------------------------------------------------------------------------------------------------------------------------------
### To set up your Git identity on your computer:
(In most cases, you should use the same email address for both Git and GitHub. You should use the same name and email address that you use for your GitHub account.)
1. Open Git Bash (a Windows application installed with Git For Windows) or the Terminal application (macOS or Linux).
2. Run the command to set your username:

		git config --global user.name "username"

3. Run the command to set your e-mail address:

		git config --global user.email "email@domain.com"

Replace "Your Name" and "your.email@example.com" with your actual name and email address. 

An example of this is:
```
git config --global user.name "Caitlin Stuart"
git config --global user.email "cstuart@email.com"
```
