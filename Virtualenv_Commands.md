# Basic Virtualenv & Virtualenvwrapper Commands

#### Virtualenv
```sh
# Create an isolated Python environment
$ cd PROJECT_FOLDER
$ virtualenv PROJECT_NAME

# Create an isolated Specific Python environment
$ virtualenv -p /usr/bin/python3.6 PROJECT_NAME 

# Activate a environment
$ source PROJECT_NAME/bin/activate

# Deactivate the environment
$ deactivate

# Delete the environment
$ rm -rf PROJECT_FOLDER         # delete a virtual environment, just delete its folder
```

---

#### Virtualenvwrapper

```sh
# Create a environment
$ mkvirtualenv ENV_NAME

# Duplicate a environment
$ cpvirtualenv ENV_NAME_OLD ENV_NAME_NEW

# Delete a environment
$ rmvirtualenv ENV_NAME

# Show details of a environment
$ showvirtualenv ENV_NAME

# List all environments
$ lsvirtualenv

# Activate a environment
$ workon ENV_NAME

# Deactivate the environment
$ deactivate
```
