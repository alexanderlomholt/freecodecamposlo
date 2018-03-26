# Git Guide

This is the FCC Oslo documentation/cheatsheet for Git.
Please read before you contribute to the project.


## Git version control

To start adding to this project you need to have Git installed.

To check if you have Git open your terminal and type
```shell
$ git --version
```

  --> Download Git [here](https://git-scm.com/downloads "Git download")


## Git commands

Git command | description
--- | --- | ---
`git init` | *initialize git in the current directory*
`git add -A` | *Adds all changes to made*
`git commit -m "message describing change"` | *initializes git in your current folder*
`git pull origin master` | *pulls latest version of repo from Github*
`git push origin master` | *push changes to master. NEVER DO THIS HERE.*
`git checkout -b name-of-branch` | *create and change to new branch*
`git checkout another-branch` | *change from current branch to another branch*
`git checkout master` | *change to master branch*
`git branch` | *see list of all local branches on your machine*
`git log` | *see list of previous commits*
`git checkout 0d1d7fc32` | *temporarily change to previous commit/version using 10 digits of commit id from git log*
`git reset --hard 0d1d7fc32` | *destroy any local modifications and revert to previous commit*
`git revert HEAD~3` | *revert back x number of times, in this case 3 commits back*
`rm -rf .git` | *remove Git entirely from current directory*


    --> For the complete Git documentation [click here](https://git-scm.com/doc, "Git documentation")


## Git workflow for FCC Oslo

...to be added.
