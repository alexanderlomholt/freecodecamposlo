# Git Guide

This is the FCC Oslo documentation/cheatsheet for Git.
Please read before you contribute to the project.

  If you do not have a github account go create one [now](https://github.com/ "Github.com")


## Git version control

To start adding to this project you need to have Git installed.

To check if you have Git open your terminal and type
```shell
$ git --version
```

  --> Download Git [here](https://git-scm.com/downloads "Git download")


## Git commands

`$ git init`  *initialize git in the current directory*

`$ git add -A`  *Adds all changes to made*

`$ git commit -m "message describing change"`  *initializes git in your current folder*

`$ git pull origin master`  *pulls latest version of repo from Github*

`$ git push origin master`  *push changes to master. NEVER DO THIS HERE.*

`$ git checkout -b name-of-branch`  *create and change to new branch*

`$ git checkout another-branch`  *change from current branch to another branch*

`$ git checkout master`  *change to master branch*

`$ git branch`  *see list of all local branches on your machine*

`$ git log`  *see list of previous commits*

`$ git checkout 0d1d7fc32`  *temporarily change to previous commit/version using 10 digits of commit id from git log*

`$ git reset --hard 0d1d7fc32`  *destroy any local modifications and revert to previous commit*

`$ git revert HEAD~3`  *revert back x number of times, in this case 3 commits back*

`$ git diff`  *difference between current and previous code*

`$ rm -rf .git`  *remove Git entirely from current directory*


For complete Git documentation [click here](https://git-scm.com/doc "Git documentation")


## Start contributing to the FCC Oslo project

First things first, you need to provide your Github username to [alexanderlomholt](https://github.com/alexanderlomholt "Alexanderlomholt Github") at our monday meetup or via the [Facebook page](https://www.facebook.com/groups/free.code.camp.oslo/ "FCC Oslo facebook page") so you can be added as a collaborator.

Next, once added as a collaborator you will receive an email from Github with instructions on how to pull the latest version of the repo to your local machine, so you can start adding to the project.

Congrats! You now have a local copy of the repo and you can start adding your code to the project and push to Github. See the next section and follow our workflow.


## Git workflow for this project

*Rule number one: do not push to the master branch :)*

*For every feature/file/change you want to make, you will create a branch before you write any code. You will then add your changes in git, make one or more commits and push the branch to Github.*

How to add some code, documentation, new files/directories etc:

```shell
$ git checkout -b name-of-new-feature-or-change
```

You are now on a newly created branch! Start writing your code/add files etc. Then:

```shell
$ git status
$ git add -A
$ git commit -m "added new button with email:to"
$ git push origin name-of-new-feature-or-change
```

Type your password when prompted.

Go to the FCC Oslo repo and click on branches. You will see your branch there, click on open pull request and wait for someone to review your code and merge it to master. Once your code has been merged you need to go fetch the updated version of the repo with your changes implemented. Back to your command line and type:

```shell
$ git pull origin master
```

Now, pull the updated master from you command line / terminal, open the index.html in your browser and make sure new changes are working as intended. If there's a bug you can create a new branch and fix it.


## Review and merge other peoples code

You can review other peoples code (pull requests) by navigating to branches on our Github repo and clicking open on a newly added branch. You can then review the code and if it looks good click on merge to master.

Now, pull the updated master from you command line / terminal, open the index.html in your browser and make sure new changes are working as intended. If there's a bug you can create a new branch and fix it.


## Creating a new Git and Github repository

You can easily create a new Github repo in your terminal/command line using [Hub](https://hub.github.com/ "Hub") which you need to install on your machine. On Mac OS you should install the [Brew](https://brew.sh/ "Brew for OSX") package manager before you install Hub.

*Create a new git project via your terminal*

```shell
$ mkdir newprojectname
$ git init
$ git touch readme.md (you need an initial file, like a readme, to push project to github)
$ git add -A
$ git commit -m "initialize project"
$ hub create
$ git remote -v
$ git push origin master
```

Now check that you new shiny repo is on your github account with the readme file you created. You're ready to start using the git workflow documented above this section.















