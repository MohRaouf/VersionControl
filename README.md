#  <p align="center"> Lab 2 - Version Control Course </p>
![Changelog](https://img.shields.io/badge/Changelog-latest-blue.svg)
## Create a new Project on my local machine
- `git init`
- `git add .`
- `git commit -m "Repo Creation - Adding my CV and README File"`

## Push it to a remote repo
- `Create a remote Repo`
- `git remote add origin git@github.com:MohRaouf/VersionControl.git`
- `git branch -M master`
- `git push -u origin master`

## Create two branches ( dev - test ) 
- `git branch dev`
- `git btanch test`

## Create two files in dev branch
- `git checkout dev`
- `touch file1 file2`
- `git add .`
- `git commit -m "Add 2 files in dev branch"`

## Push changes to the remote repo
- `git push origin dev` 
- `git push origin test`

## Merge these changes on the master branch
- `git checkout master`
- `git merge dev`

## Create a temp branch and push it to the remote repo
- `git checkout -b tempBranch`
- `git push origin tempBranch`

## Remove the branch from local repo
- `git checkout master`
- `git branch -d tempBranch` if the branch is published to the remote repo
- `git branch -D tempBranch` force deletion even if it's not published yet

## Remove the branch from remote repo
- `git push origin --delete tempBranch`  
    or 
- `git push origin :tempBranch`

## Send Invitation to Eng. Maha
<p align="center">
    <img src="https://github.com/MohRaouf/VersionControl/blob/master/invitation.png" alt="Invitation" />
</p>

## Create an annoted tag with tagname v1.4
- `git tag -a v1.4 -m "Secomd Release"`

## Push tag to remote repo
- `git push origin v1.4`

## List the local tags
- `git tag`

## delete tag from local repo 
- `git tag -d v1.0`

## delete tag from remote repo 
- `git push origin :refs/tags/v1.0`

## What is git rebase?
- Rebasing is the process of moving or combining a sequence of commits to a new base commit. 
  Rebasing is most useful and easily visualized in the context of a feature branching workflow.

## Rebase Example
- `git checkout master`
- `git add .`
- `git commit -m "Add pullRequest Img - Fill Command.txt"`
- `git push origin master` 
- `git checkout dev` 
- `git rebase master`
- `git push -f origin dev` 


## Make a pull reguest
<p align="center">
    <img src="https://github.com/MohRaouf/VersionControl/blob/master/pullRequest.png" alt="Pull Request" />
</p>

## README File containing IMG
- Done




