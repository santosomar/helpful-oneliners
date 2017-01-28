# Helpful One line Scripts
This is just a collection of helpful one line scripts for Linux utilities, miscelaneous tasks, etc.
Feel free to contribute and add your own.

## Cleaning up /boot in Linux
This is useful to automatically clean /boot in Linux.
```
apt-get remove `dpkg --list 'linux-image*' |grep ^ii | awk '{print $2}'\ | grep -v \`uname -r\``
```
