# General npm Commands

```sh
$ npm -v                                    # view npm version
$ npm i -g npm

# Help
$ npm help
$ npm help update
$ npm help npm                              # involived overview
$ npm COMMAND -h                            # quick help on the command
$ npm help-search update
```
---

### Install npm Package
```sh
# Install Package
$ npm install PACKAGE_NAME                  # install package locally
$ npm install PACKAGE_NAME -h               #
$ npm install PACKAGE_NAME -g               # install package globally
$ npm install PACKAGE_NAME --save           # save the package depends on
$ npm install PACKAGE_NAME --save-dev
$ npm install PACKAGE_NAME@3.2.1 --save     # save a specific version

# Uninstall Package
$ npm uninstall PACKAGE_NAME
$ npm uninstall PACKAGE_NAME -g
$ npm uninstall PACKAGE_NAME --save
$ npm uninstall PACKAGE_NAME --save-dev
$ npm uninstall *                           # delete all local npm package inside node_modules folder

# Prune Package
$ npm prune

# Update Package
$ npm update -g                             # update globally
$ npm update PACKAGE_NAME --save

# List Package
$ npm list
$ npm list --depth 0
$ npm list --global true --depth 0
```
---

### Create nmp Module
```sh
# Initilse
$ npm init
$ npm init --yes                            # npm init -y (shortcuts)

# Config
$ npm config ls
$ npm config get prefix

$ npm config set init-author-name "NAME"
$ npm set init-license "MIT"
$ npm init --yes

$ npm config get init-author-name
$ npm get init-license

$ npm config delete init-license
$ npm config delete init-author-name

# Publish Module
$ npm adduser
$ npm publish

$ npm version patch
```
