# Bandit Level 8 → Level 9

[url](https://overthewire.org/wargames/bandit/bandit9.html)

## Level Goal

The password for the next level is stored in the file **data.txt** and is the only line of text that occurs only once

```
$ cat data.txt | strings | sort | uniq -u
UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR
# close ssh connection
$ ssh bandit9@bandit.labs.overthewire.org -p 2220
# type password
```

## Flag

`UsvVyFSfZZWbi6wgC7dAFyFuR6jQQUhR`