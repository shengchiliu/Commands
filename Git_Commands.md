# Basic Git Commands

#### Initial setting
```sh
$ git config --global user.name "USERNAME"
$ git config --global user.email "USERNAME@EMAIL.COM"
```
#### Cache your GitHub password in Git if you using Linux (Optional)
```sh
$ git config --global credential.helper cache                   # password cached by default 15 minutes
$ git config --global credential.helper 'cache --timeout=3600'  # set a longer timeout, 1 hour
```
--------------------------------------------------------------------------------
#### Create a new repository
```sh
# 1. Add a new repository on your GitHub
# 2. And then type the following commands in your Terminal

$ echo "# REPOSITORY" >> README.md
$ git init
$ git add README.md
$ git commit -m "initial commit"
$ git remote add origin https://github.com/USERNAME/REPOSITORY.git
$ git push -u origin master
```
#### Clone a existing repository
```sh
$ git clone https://github.com/USERNAME/REPOSITORY.git
$ git pull
```
--------------------------------------------------------------------------------
#### Update your repository
```sh
# After creating your repository, you can update your repository after coding.
$ git status                            # show your git status
$ git add .                             # add all the files you modified/added in git index
$ git commit -m "YOUR COMMENT"          # saved in your local repository
$ git push -u origin master             # update to your remote repository
```

#### Rename a file in your repository
```sh
$ git mv OLD_FILE_NAME.XXX NEW_FILE_NAME.XXX
$ git commit -m "YOUR COMMENT"
$ git push -u origin master
```

#### Remove a file in your repository
```sh
$ rm -rf FILE_NAME.XXX
$ git rm FILE_NAME.XXX
$ git commit -m "YOUR COMMENT"
$ git push -u origin master
```
#### Remove a file only from your repository and not remove it from your filesystem
```sh
$ git rm --cached FILE_NAME.XXX
$ git commit -m "YOUR COMMENT"
$ git push -u origin master
```
--------------------------------------------------------------------------------
#### Commands about branch
```sh
$ git branch                            # list all branches
$ git branch BRANCH_NAME                # create a new branch
$ git checkout BRANCH_NAME              # switch a branch to another
$ git checkout -b BRANCH_NAME           # create and then switch branch
$ git branch -d BRANCH_NAME             # delete a branch
```
#### Change to a new remote's URL
```sh
$ git remote -v                         # show the remote GitHub URL
$ git remote set-url origin https://github.com/USERNAME/REPOSITORY.git
```
--------------------------------------------------------------------------------
#### Work with others in the same repository
```sh
$ git clone https://github.com/USERNAME/REPOSITORY.git      # download your team's repository
$ git pull
$ git branch BRANCH_NAME                                    # create a new branch (avoid to use master)
$ git checkout BRANCH_NAME

# update your code to the repository after your coding
$ git add .
$ git commit -m "YOUR COMMENT"
$ git push -u origin BRANCH_NAME
```
--------------------------------------------------------------------------------
#### Delete a repository's commit history in Github
```sh
$ rm -rf .git                           # all commit history will be gone, so you may need to backup
$ git add .
$ git commit -m "YOUR COMMENT"
$ git remote add origin https://github.com/USERNAME/REPOSITORY.git
$ git push -u --force origin master
