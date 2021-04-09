Notes from class 3, using git. 

Prior to git, I imagine developers jumped out of windows because the possiblity of catestrophic losses was possible. 
Below are many of the notes from udemy's class about git--very specifc keystrokes to correctly code within git.

Another beuty of git is that you can work in the cloud or locally on your own machine. 

You clone repositories, work locally, then add/commit/push to place them into the cloud.

There is also an undo function--thank God. That is by using the -amend command.

The primary sequence is add/commit/push. But one can stash changes prior to committing--it temporarly removes changes and hides them with a clearn working direlcy. 
When you're ready to continue, you use 'git stash apply' to retrieve the hidden changes.

History of Git
Git traces its roots to the open source software project Linux kernel. Developers of this project began using a DVCS called BitKeeper in 2002. In 2005, many of these developers stopped using this DVCS due to tension between the Linux kernel community and the company behind BitKeeper’s and the eventual revocation of the DVCS’ gratis status. Subsequently, Linus Torvalds, the chief architect of the Linux kernel, began creating Git. With the intention of creating a DVCS with a workflow design similar to that of BitKeeper, which was also fast, Git allowed for non-linear development via multiple branches, could support large projects, possessed strong mechanisms preventing corruption, and had a simple design. Since its inception in 2005, Git has become one of the most utilized Version Control Systems in the world.

Mac OS X
Terminal

The simplest method for installing Git on a Mac (for Mavericks 10.9 and above) is running Git from the Terminal. If Git is not installed, you will see a prompt for installation.

Git Website

You can also download Git by visiting this link and following the posted directions:

http://git-scm.com/download/mac

GitHub

A third option is to install Git as part of the GitHub for Mac install. GitHub is repository hosting service, which we will discuss in a future section.

Download GitHub for Mac via the following link:

http://mac.github.com

Graphical Clients
Git includes inherent Graphical User Interface (GUI) tools. However, users can also utilize third-party tools created for particular platforms.

GUI Clients

You can access a variety of GUI clients for Mac, Windows, and Linux via the following link:

https://git-scm.com/downloads/guis

Initial Customization
After making sure Git has been installed, you should perform some customization steps, which should only need to be completed once on any machine. To change settings, you can repeat these steps.

Configuration of Variables

An inherent Git tool called git config allows the setting of configuration variables that control aspects of Git’s operation and look.

Identity Setting

After installing Git, users should immediately set the user name and email address, which will be used for every Git commit.

Type the following into Terminal or Command Line:

git config --global user.name "Jane Smith"

git config --global user.email "example@email.com"
To confirm that you have the correct settings, enter the following command:

git config --global user.name (should return Jane Smith)

git config --global user.email (should return example@email.com)
*By using the –global option, these Git settings apply to anything on the system. To use different identity settings for a specific project, change the working directory to the desired local Git repository and repeat the steps above without using –global.
Check Settings
To check settings, use the git config --list command.

Example:

$ git config --list

user.name=Jane Smith

user.email=example@email.com

color.status=auto

color.branch=auto

color.interactive=auto

...
Getting Help
There are three ways to get more information on a particular command, by accessing the manual:

git help command

git command --help

man git-command
Setting up a Git Repository
Importing
To import an existing project or directory into Git, follow these steps using the Terminal or Command Line:

Switch to the target project’s directory
Example:

$ cd test (cd = change directory)
Use the git init command
$ git init
Note: At this stage, you have created a new subdirectory named .git that has the repository files. Tracking has not commenced.

To start tracking these repository files, perform an initial commit by typing the following:
$ git add *.c
$ git add LICENSE
$ git commit -m “any message here”
Now, your files are tracked and there’s an initial commit. We will discuss the particular commands in detail soon.

Cloning
You can also create a copy of an existing Git repository from a particular server by using the clone command with a repository’s URL:

$ git clone https://github.com/test
By cloning the file, you have copied all versions of all files for a project. This command leads to the creation of a directory called “test,” with an initialized .git directory inside it, which has copies of all versions of all files for the specified project. The command also automatically checks out — or retrieves for editing — a copy of the newest version of the project.

To clone a repository into a directory with another name of your choosing, use the following command format:

$ git clone https://github.com/test mydirectory
The command above makes a copy of the target repository in a directory named “mydirectory.”

Workflow
Local Repository Structure
The local Git repository has three components:

Working Directory: The actual files reside here.
Index: The area used for staging
Head: Points to the most recent commit
image03

Saving Changes
All files in a checked out (or working) copy of a project file are either in a tracked or untracked state.

Tracked

Tracked files can be modified, unmodified, or staged; they were part of the most recent file snapshot.

Untracked

Untracked files were not in the last snapshot and do not currently reside in the staging area.

*After cloning a repository, files have tracked status and are unmodified because they have been checked out but not edited.

The Life Cycle of File Status
After you edit a file, Git flags it as modified because of changes made after the previous commit.
You stage the modified file.
Then, you commit staged changes.
Tracking and Staging a New File
Single File

Track one file only by using the following format:

git add filename
All Files

Track all files in a repository by using the following command:

$ git add *
*After using these commands, files are tracked and staged for committing.

After adding a new file called EXAMPLE, you would see information regarding changes to be committed when using the git status command:

$ git status

On branch master

Changes to be committed:

  (use "git reset HEAD ..." to unstage)
new file: EXAMPLE
This information tells us that there are changes to be committed and that the file has been staged.

Committing a File
After staging one or multiple files, you should commit the changes and record what you did within the commit message:

$ git commit -m “made change x,y,z”
*This step has committed changes for the file or files (you can have one commit message for multiple files, if applicable) to the HEAD.

Committing All Changes
$ git commit -a
*This command commits a snapshot of all modifications to tracked files in the working directory.

Pushing Changes
Next, you would push changes to a remote repository. We will discuss remote repositories in more depth in the next section. For now, we will look at a general overview of pushing changes to remotes.

Example:

$ git push origin master
*This command pushes changes from the local “master” branch to the remote repository named “origin”.

*For cloned repositories, Git will automatically give the name “origin” to the server from which you cloned and the name “master” to your local repository. However, these names can be changed by the user.
Undoing Actions
Git has mechanisms for undoing certain actions.

Commit Mistakes
You can use the –amend command when you need to alter a commit message or forgot to add some files.

$ git commit --amend
In the example above, you can use this command to easily change your commit message, if no changes were made since the newest commit.

$ git commit -m “my first commit”

$ git add example_file

$ git commit --amend
In the above example, a forgotten file is added to a commit.

Unstaging a File
$ git reset HEAD index.html

Unstaged changes after reset:

M index.html
Above, we see that the git reset HEAD command unstaged the index.html file.

NOTE: When git reset --hard is used, Git overwrites all changes in the working directory, permanently destroying any uncommitted changes.
