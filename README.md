# FirstTest
Nada. Just for testing


Now we're on a protected master.  
Must use pull request.  

Default branch renamed from master to main on github.  
Locally cloned repo can be updated with following:  
```
git branch -m master main          # move (rename) local master to main
git fetch origin -p                # fetch the new branch and prune old master (origin/HEAD has become dangling)
git branch -u origin/main main     # set-upstream-to origin/main
git remote set-head origin -a      # Updates the remote default branch (--auto). In .git/refs/remotes/origin/HEAD
```

Do stuff that is going to be reverted.
1. branch
2. commit changes
3. git tag revert-ref
4. git reset --hard HEAD~1
5. git reset --soft revert-ref    ## or HEAD@{1}
6. git commit -a -m "reverted...."
7. git tag --delete revert-ref
