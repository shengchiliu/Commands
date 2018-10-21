# Commands for Linux System

## Show System Information

```sh
# Show all DMI table contents:
sudo dmidecode

# Show the BIOS version:
sudo dmidecode -s bios-version

# Show the system's serial number:
sudo dmidecode -s system-serial-number

# Show BIOS information:
sudo dmidecode -t bios

# Show CPU information:
sudo dmidecode -t processor

# Show memory information:
sudo dmidecode -t memory
sudo dmidecode --type 17 | grep Size
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

---
