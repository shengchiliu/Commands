# Install ttyecho

1. Download ttyecho.c
2. $ make ttyecho
3. $ sudo mv ttyecho /bin/

# ttyecho Commands
```sh
# Send Commands to a tty Terminal
sudo ttyecho -n /dev/ttys001 COMMANDS

# End a Process (ctrl+c) (Echo Control a C Character)
sudo ttyecho -n /dev/ttys001 echo $'\cc'

# Send a echo Escape Characters (ESC)
sudo ttyecho -n /dev/ttys001 echo -e

```
