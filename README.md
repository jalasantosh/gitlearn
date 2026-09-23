# gitlearn
This is to setup Git and learn basics

git config --list  -- to list all users 
create a working directory : for ex mkdir gitpractice  (and then intialize with below command.)
If u want to initialize a particular working directory : git config --global alias.i init


Step 1:
push
pull 
fetch

GIT COMMANDS :

Git stash : stores/saves  your data

stash commands:
git stash
git stash apply
Any particular stash to apply : git stash apply stash@{0 or 1}

Git Stash Command
The git stash command is used to temporarily save changes in your working directory that you are not ready to commit yet. It allows you to clean your working directory without losing your changes, so you can work on something else and come back to your changes later.

Basic Usage

To stash your changes, simply run: git stash

Copy : This command saves your local modifications and reverts the working directory to match the HEAD commit. By default, the stash is listed as "WIP on branchname ...", but you can provide a custom message:
git stash push -m "Custom message"

Listing Stashes : 
To see a list of all stashed changes, use:

git stash list

Each stash entry is listed with its name (e.g., stash@{0} for the latest entry) and a short description of the commit the entry was based on.

Applying Stashes :

To apply the most recent stash, use: git stash apply

To apply a specific stash, specify its name: git stash apply stash@{1}

If you want to apply and remove the stash from the list, use:
git stash pop


If you want to create a new branch from a stash, use: git stash branch <branchname>

Other Useful Commands

Show Stash: To see the changes recorded in a stash entry: git stash show -p stash@{0}
Drop Stash: To remove a specific stash entry: git stash drop stash@{0}
Clear Stashes: To remove all stash entries: git stash clear


Notes :
git stores all the global configurations in : .gitignore file
types of repos : local and remote.
Git hub : web-based platform
git bash is a : command line interface

-------------- Important commands :

status of a repo : git status
check history of logs : git log
forcefully delete a branch : git branch -d
show differences : git diff
To add all files of current directory to staging area : git add --all
To verify git settings  of a local repo : git config --list
Command to fetch down changes from global repo : git fetch
to make copy of a real repo : git fork

Q1. I want to make a new branch with branch-name gfg from a specific tag name quiz, write a command will be used to create a new branch.
git checkout -b gfg quiz

Q2. Command to update a branch with the latest changes.
git pull

Q4. Write a command which create a new commit by combining the changes in one branch with another branch.
git merge


Q5. Write a command using which a new commit will be created when you integrate the changes.
git rebase

Q6. Write a command to delete untracked files in git working directory.
git clean

Git Merge and Rebase :

