# gitlearn
This is to setup Git and learn basics


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
1
2
3
The git stash command is used to temporarily save changes in your working directory that you are not ready to commit yet. It allows you to clean your working directory without losing your changes, so you can work on something else and come back to your changes later.

Basic Usage

To stash your changes, simply run:

git stash
Copy
This command saves your local modifications and reverts the working directory to match the HEAD commit. By default, the stash is listed as "WIP on branchname ...", but you can provide a custom message:

git stash push -m "Custom message"
Copy
Listing Stashes

To see a list of all stashed changes, use:

git stash list
Copy
Each stash entry is listed with its name (e.g., stash@{0} for the latest entry) and a short description of the commit the entry was based on.

Applying Stashes

To apply the most recent stash, use:

git stash apply
Copy
To apply a specific stash, specify its name:

git stash apply stash@{1}
Copy
If you want to apply and remove the stash from the list, use:

git stash pop
Copy
Creating a Branch from a Stash

If you want to create a new branch from a stash, use:
git stash branch <branchname>

Other Useful Commands

Show Stash: To see the changes recorded in a stash entry: git stash show -p stash@{0}

Drop Stash: To remove a specific stash entry: git stash drop stash@{0}
Clear Stashes: To remove all stash entries: git stash clear


