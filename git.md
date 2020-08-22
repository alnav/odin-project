# GIT

### Commands

* ```git init```  start repository
* ```.gitignore``` file
    * add files to ignore, e.g. ```.project *.pyc```
* ```git status``` shows state of working directory and staging area
* ```git add -A``` add all files to staging area
* ```git reset *fileName*``` removes files from stagin area
* ```git commit -m "commit message"``` commit to repository
* ```git log``` review changes made
* ```git clone <url>``` cloning a remote repository
* ```git remote -v``` list information on repository
* ```git branch -a``` list branches (both local and remote) of repository
* ```git diff`` shows difference made to files

## Pushing changes
**Commit changes**
```
git diff
git status
git add -A
git commit -m "new changes made"
```
**Push changes**
```
git pull origin master
git push origin master
```
* ```git pull``` necessary if working with other users

## Common workflow
### Create a branch for feature
  
```
git branch new-feature
git checkout new-feature
```
* ```git branch``` create new branch
* ```git checkout``` switch to branch

### Push branch to remote
```
git push -u origin new-feature
git branch -a
```
```git branch -a``` shows all branches

### Merge a branch
```
git checkout master
git pull origin master
git branch --merged 
git merge new-feature
git push origin master
```

### Delete a branch
```
git branch --merged
git branch -d new-feature
git branch -a
git push origin --delete new-feature
```
* branch can be deleted after push

