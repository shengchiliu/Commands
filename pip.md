# General pip Commands
```sh
# Upgrade Package
$ pip install --upgrade pip
$ pip install --upgrade PACKAGE

$ python2 -m pip install --upgrade PACKAGE
$ python3 -m pip install --upgrade PACKAGE

# Install Package
$ pip install PACKAGE
$ python2 -m pip install PACKAGE            # install Python2 module
$ python3 -m pip install PACKAGE            # -m calls __main__.py module of a specified package

# List Packages
$ pip list
$ python2 -m pip list
$ python3 -m pip list

# Search Package
$ pip search PACKAGE
$ python2 -m pip search PACKAGE
$ python3 -m pip search PACKAGE

---

# Create Requirements File
$ pip freeze > requirements.txt             # list Python dependencies in the file

# Install Python Packages from Requirements
$ pip install -r requirements.txt

```
