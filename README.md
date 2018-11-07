# Hands On Lab November 2018

## Posh-git

https://github.com/dahlbyk/posh-git

Modifies the PowerShell prompt to include the git status.
Adds Tab Completion of git commands
Some SSH capabilities
Update all branches command

Open a PowerShell command window and enter the following

```
install-module posh-git

```

After posh-git has been installed you can import the module.

```
Import-Module posh-git

```

If you want posh-git to be available all the time you can enter the following command

```
Add-PoshGitToProfile

```

If you go to a directory that contains a git repo you should see the prompt change to the current status of that repo.

## VS Code

Visual Studio Code is tightly integrated with Git.

Open Visual Studio without any project. On the left hand side of the screen you should be able to see the Source Control Management (SCM) panel.
Open the command palette (ctrl-shift-P) and type **Git**. You will see several Git commands availalbe.

Select or type the clone command (git clone)
You will be presented with a text box that allows you to enter a repos URL.
Enter the url from the Phillydotnet git repo for this lab.
You will be prompted for a location to put the repo. The repo will be place into a subdirectory under the directory you select.
After the repo downloads you will get a dialog asking if you would like to open the repo. CLick the Open Respostory button.

At thsi point you may be asked to log into Github.com. If you are, then click the _Sign in_ button.

You should now have a directory with the repo in it.

Assuming you have installed posh-git and had it added to always load, you should be able to open a command prompt from within VS Code and posh-git should be working.

Make some changes to the readme file - save it - then go back to the command prompt and see what happens when you hit the enter key.

On the left side of the screen you should see a number in the SCM button. Click on it and you should see the readme file listed with an M (for modified).
There is a text box at the top of the pane, enter a commit message and then hit the check mark (or Ctrl-Enter).
A dialog box will open asking if you want to stage and commit the changes, click Yes.

At the bottom of the screen in the status bar you should see a double arrow in a circle with numbers and arrows next to them. Click on this and you will synchronize your changes.
You may be asked to log into github again, if so, log in and continue.

With the SCM still open, hover over the bar above the textbox and you should see an elipse. Click on the elipse. You should see lots of git commands.

In the status bar you can see the branch name - it should be master.
Click on the name and you will get an option to create a branch.
Click on create a new branch and it will prompt you for a name. Name it anything you want. Spaces will be turned into hyphens.

## Extensions

Also on the left is the VS Code Extensions pane. Click on it to open it.
Enter Git into the search box and you should see a list of git extensions - we are not going to be going over all of them.

### GitLens

This is one of my favorite extensions for git. It adds a pane on the left and also shows

### Git Blame

This one adds "blame" information in the status bar.

### Git History

This allows you to show a visual history of the branches and commits.
