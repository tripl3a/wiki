# Git commands

## New repository

```
cd git-reps
mkdir wiki
git init wiki

cd wiki
git remote add origin https://github.com/tripl3a/wiki.git
git pull origin master
```

## Add stuff

```
# commit all changes:  
git commit -a
# Push the changes in your local repository to GitHub:
git push origin master
```

## Remove stuff

```
# unversion a file
git rm --cached <filename>
```