# Basic Conda Commands

### Update Conda
```sh
$ conda update conda
$ conda update --all
```
---
### Commands for Environment
```sh
# List Environments
$ conda info --envs                                                     # --envs or -e

# Create Environment
$ conda create --name ENVIRONMENT_NAME                                  # --name or -n
$ conda create --name ENVIRONMENT_NAME python=3.5                       # create a specific python environment
$ conda create --name ENVIRONMENT_NAME_NEW --clone ENVIRONMENT_NAME_OLD # clone an environment

# Activate/Deactivate Environment
$ source activate ENVIRONMENT_NAME		                                # (Windows) activate ENVIRONMENT_NAME
$ source deactivate	                                                    # (Windows) deactivate

# Delete Environment
$ conda remove --name ENVIRONMENT_NAME --all
```
---
### Commands for Package
```sh
# List Package
$ conda list

# Install Package
$ conda install --name ENVIRONMENT_NAME PACKAGE_NAME                    # install in a specific environment
$ conda install PACKAGE_NAME                                            # install in the current environment

# Remove a package
$ conda remove --name ENVIRONMENT_NAME PACKAGE_NAME                     # remove in a specific environment
$ conda remove PACKAGE_NAME                                             # remove in a specific environment

# Search Package
$ conda search PACKAGE_NAME                                             # Show Python Versions
$ conda search --full-name python
```
