# GitHub Notes

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