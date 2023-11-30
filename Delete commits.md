How to delete commits from a branch in Git?

Deleting a commit in Git must be approached in one of two ways, depending on if you have or have not pushed your changes. **Please note before attempting this, running these commands will DELETE your working directory changes.** Any changes to tracked files in the working tree since commit are discarded. Be sure to separately save any changes you'd like to have.  
      
If your changes have **not been pushed** yet simply enter the command 

`git reset --hard HEAD~1

This will discard all working tree changes and move HEAD to the commit before HEAD.  
  
If you'd like to delete the commits up until a specific commit, running `git log` into the command line to find the specific commit id and then running

`git reset --hard sha1-commit-id

will discard all working tree changes and move HEAD to the commit chosen.
 
Alternatively, if you **have** **already pushed** your changes you will need to run the following code

`git push origin HEAD --force 

Please note if others have pulled this branch you would be better off starting a new branch. If you don't do this when someone else pulled, it will just merge it into their work, and you will get it pushed back up again.  
      
_If you need to find a commit that you "deleted", it is typically present in <_git reflog> _unless you have garbage collected your repository_