# FirstTest
Nada. Just for testing


Now we're on a protected master.  
Must use pull request.  

Dafault branch renamed from master to main on github.  
Locally cloned repo can be updated with following:  
```
git branch -m master main          # move (rename) local master to main
git fetch origin -p                # fetch the new branch and prune old master (origin/HEAD has become dangling)
git branch -u origin/main main     # set-upstream-to origin/main
git remote set-head origin -a      # Updates the remote default branch (--auto). In .git/refs/remotes/origin/HEAD
```
