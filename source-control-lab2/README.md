# Removing Branches in Git



## To Remove a Branch Locally

1. Switch to a different branch:

   in git bash
   git checkout main 
Delete the local branch:

For branches with no unmerged changes:

#Bash

git branch -d <branch-name>  
For branches with unmerged changes (use with caution):

#Bash

git branch -D <branch-name> 
To Remove a Branch Remotely
Delete the branch from the remote repository:

#Bash

git push origin --delete <branch-name>  
Verify Branch Deletion
Verify locally:

#Bash

git branch 
##The deleted branch should not appear in the list

Verify remotely:

#Bash

git branch -r 
##The deleted branch should not appear in the list