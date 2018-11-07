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
