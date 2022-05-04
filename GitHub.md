# GitHub Notes

## Common
`git status` list which unstaged files have changed
`git diff` list (unstaged) changes to files
`git log` list recent commits

## New Repo from command Line
```sh
$ gh repo create
```

## Setting up a new Git Repo


### Create a new local repo and push to remote

    touch README.md
    git init
    git add README.md
    git commit -m "first commit"
    git remote add origin git@github.com:alexpchin/<reponame>.git
    git push -u origin main
    
### Push an existing repository from the command line

    git remote add origin git@github.com:alexpchin/<reponame>.git
    git push -u origin main

### Create a new branch from an earlier commit

```shell
git branch <branchname> [<commit-id>]
```


### Delete a branch

```shell
git branch -d <branchName>
```

Example:
```shell
git branch new-feature-branch e6f99e34861b0a1558351162c4ac867e0d8a807e
```

### Show a list of all commits

```shell
git log --oneline
```

### Show a list of all branches

```shell
git branch
```


# HUGE ONE!!  

`git merge main` when on branch after pulling from main

# Merging Branch back to main
`git checkout main` checkout main branch
`git merge branchname` merge branch into main


### Branches on Remote
`git branch` list currently existing branches (local)
`git fetch origin` get information on all remote branches to display on local
`git branch -r` show remote branches
`git branch -r --no-merged` show unmerged remote branches
