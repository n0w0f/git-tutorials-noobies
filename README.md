# Git & Github Tutorial !

git init

git add .

git reset . 

git status


## commit

 git commit -m "initial commit"

 git log

## VS Code 
  git lense
  git source control

## Git remote

git remote add origin <git url>



## Git Push

git push origin master -u 
-u (set origin to upstream remote)


## Git Merge

Fast-Forward
git fetch
git merger origin/master   (merge origin/master on top of our code in local branch)

## Git Pull
git pull (git fetch + git merge)

 - stash / commit if local has additional changes made
 - merge conflicts 

## Git clone

## Git codespace

enter period command in repo
.

## Git Branch

git branch (list all branch)

git branch -M main

git branch awesome

### Delete branch
git branch -d awesome (delete only if not merged / or no changes)
git branch -D awesome

## Git checkout

git checkout -b awesome
git branch awesome + git chekout awesome 

git checkout - (take you to previous branch)


## merge conflicts

I am also working on this line !!

if we are in master and want to merge awesome to master
git merge awesome


## git Fork

own version of project on ypur github
make changes without affecting original repo (upstream repository)
make PR from github to original

## Pull request
1. fork the repo
2. clone the fork
3. develop in local , in a new feat branch
4. commit and push
5. make a pull request

when working with fork locally we can keep it in sync with the original

git remote add upstream < git url>
git fetch upstream
git rebase upstream/master 

## Git reset

working dir , staging dir , commit

 git add . --> takes to staging area
 git reset  --> unstage changes

 




