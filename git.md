# Basic Git Commands

### Initial Settings

```sh
$ git config --global user.name "USERNAME"                      # set up user name
$ git config --global user.email "USERNAME@EMAIL.COM"           # set up user email
$ git config --list                                             # list config settings

# Cache your GitHub password in Git (Linux only)
$ git config --global credential.helper cache                   # password cached by default 15 minutes
$ git config --global credential.helper 'cache --timeout=3600'  # set a longer timeout, 1 hour
```

---

### Commands for Repository

```sh
# Create Repository
# (add a new repository on your GitHub first, and then type the following commands)
$ echo "# REPOSITORY" >> README.md
$ git init
$ git add README.md
$ git commit -m "initial commit"
$ git remote add origin https://github.com/USERNAME/REPOSITORY.git
$ git push -u origin master

# Update Repository
$ git status                                            # show your git status
$ git add .                                             # add all modified/added files in git index
$ git commit -m "YOUR COMMENT"                          # saved in your local repository
$ git push -u origin master                             # update to your remote repository

# Clone Repository
$ git clone https://github.com/USERNAME/REPOSITORY.git
$ git clone --recursive https://github.com/USERNAME/REPOSITORY.git  # including submodules 
$ git clone --recursive -b BRANCH REPOSITORY            # clone a specific branch of repo
$ git clone --depth 1 --single-branch                   # clone a 1 history commit with only master branch
$ git clone --depth 2 --no-single-branch                # clone a 2 history commits with all branchs
$ git pull

# Rename Repository
# Rename a new repository on GitHub first
$ git remote -v                                         # view the remote GitHub URL
$ git remote set-url origin https://github.com/USERNAME/REPOSITORY.git

# Remove Repository
$ rm -rf .git                                           # delete local repository
# (and then delete the repository on GitHub, if you wish to detelte the remote repository

# Remove Repository's Commit History on Github
$ rm -rf .git
$ git add .
$ git commit -m "YOUR COMMENT"
$ git remote add origin https://github.com/USERNAME/REPOSITORY.git
$ git push -u --force origin master

# List Directory Managed by git
$ git ls-files

# Revert Git Repository to a Previous Commit
$ git log

# Reverting Working Copy to the Lost Commit
$ git reset --hard HEAD                                 # last commit in your current branch

# Reverting working Copy to an Older Commit
$ git reset YOURCOMMITCODE
$ git reset --soft HEAD@{1}                             # Moves pointer back to previous HEAD
$ git commit -m "Revert to YOURCOMMITCODE"
$ git reset --hard                                      # Updates working copy to reflect the new commit
```

---

### Commands for Files

```sh
# Update File
$ git commit -am "YOUR COMMENT"                         # update an existing file
$ git push -u origin BRANCH_NAME

# Rename File
$ git mv OLD_FILE_NAME.XXX NEW_FILE_NAME.XXX
$ git commit -m "YOUR COMMENT"
$ git push -u origin master

# Remove File
$ git rm --cached FILE_NAME.XXX                         # delete file in local repository
$ git commit -m "YOUR COMMENT"                          #
$ git push -u origin master                             # delete file in remote reporsitory
$ rm -rf FILE_NAME.XXX                                  # delete file in local system
```

---

### Commands for Branch

```sh
$ git branch                                            # list all branches
$ git branch BRANCH_NAME                                # create a new branch
$ git checkout BRANCH_NAME                              # switch a branch to another ($ git checkout v0.4.0  # back to a old version)
$ git checkout -b BRANCH_NAME                           # shorthand for create and switch branch
$ git branch -d BRANCH_NAME                             # delete a branch

# Merge Changes
$ git checkout -b BRANCH_NAME                           # create and switch to a new branch
$ git commit -am "YOUR COMMENT"                         # commit your changes
$ git checkout master                                   # switch to original branch
$ git merge -m "YOUR COMMENT" BRANCH_NAME               # merge the changes
$ git branch -d BRANCH_NAME                             # delete the new branch

# Work with Others in the Same Repository
$ git clone https://github.com/USERNAME/REPOSITORY.git  # download your team's repository
$ git pull
$ git branch BRANCH_NAME                                # create a new branch (avoid to use master)
$ git checkout BRANCH_NAME
```

---

### Commands for Commit

```sh
# Show Commit
$ git show
$ git log -1

# Amend Commit
$ git commit --amend -m "NEW COMMIT MESSAGE"              # amend the most recent commit message

# Unstage Commit (Undo git add)
$ git reset .
$ git reset -- FILE1 FILE2 FILE3
```
