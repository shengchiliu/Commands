# Commands for Linux System

## Show System Information

```sh
# Show all DMI table contents:
$ sudo dmidecode

# Show the BIOS version:
$ sudo dmidecode -s bios-version

# Show the system's serial number:
$ sudo dmidecode -s system-serial-number

# Show BIOS information:
$ sudo dmidecode -t bios

# Show CPU information:
$ sudo dmidecode -t processor

# Show memory information:
$ sudo dmidecode -t memory
$ sudo dmidecode --type 17 | grep Size
```

---

## Install deb File

```sh
$ sudo dpkg -i /path/to/deb/file
$ sudo apt-get install -f
```

## Find a Specific Word inside Text File

```sh
$ grep -r <SEARCH_WORD> *
```

## Find a Specific File

```sh
$ find ./ -name "FILENAME"
```

## Zip/Unzip File

```sh
# tgz Files
$ tar -zcvf <FILENAME>.tgz <./DIRECTORY>      # zip files
$ tar -zxvf <FILENAME>.tgz                    # unzip files

# zip Files
$ zip -r <FILENAME>.zip <FOLDER_DIRECTORY>    # zip folder
$ unzip <FILENAME>.zip -d <FILENAME_FOLDER>   # unzip files
```

## Install .tar.xz File

```sh
tar -xvf <FILENAME.tar.xz>                    # install .tar.xz file
```

## Download File

```sh
$ curl -o <FOLDER/FILENAME> -O <https://www...>
# Example, download imgcat file and chmod the file
$ sudo curl -o /usr/local/bin/imgcat -O https://iterm2.com/utilities/imgcat && sudo chmod +x /usr/local/bin/imgcat
```

---

## Shortcuts

- <kbd>Ctrl</kbd> + <kbd>A</kbd> or <kbd>Home</kbd>: Go to the beginning of the line.
- <kbd>Ctrl</kbd> + <kbd>E</kbd> or <kbd>End</kbd>: Go to the end of the line.

- <kbd>Alt</kbd> + <kbd>B</kbd>: Go left (back) one word.
- <kbd>Alt</kbd> + <kbd>F</kbd>: Go right (forward) one word.

- <kbd>Option</kbd>/<kbd>Alt</kbd> + <kbd>Left</kbd> <kbd>Right</kbd>

- <kbd>Ctrl</kbd> + <kbd>B</kbd>: Go left (back) one character.
- <kbd>Ctrl</kbd> + <kbd>F</kbd>: Go right (forward) one character.

---

## Symbolic Links

```sh
$ ln -s </path/to/file_or_folder-name> <link-name>
```

## bash or zsh

```sh
$ chsh -s /bin/zsh
$ chsh -s /bin/bash
```

## Count Files

``sh
ls | wc -l
ls /etc | wc -l
```

## Make directory if doesn't exist
```sh
mkdir -p foo/intermediate/dir
```

## Install .sh File

```sh
$ chmod +x file.sh
$ ./file.sh
```

## Display total size of a directory

```sh
$ du -hs ./directory/
```

## .bashrc at ssh login
.bashrc is not sourced when login using SSH. Need to source it in .bash_profile
```sh
if [ -f ~/.bashrc ]; then
  . ~/.bashrc
fi
```
ref. https://stackoverflow.com/questions/820517/bashrc-at-ssh-login/820533#820533

## Detector txt encording type

```
# uchardet is an encoding detector library
uchardet <FILENAME>
```
