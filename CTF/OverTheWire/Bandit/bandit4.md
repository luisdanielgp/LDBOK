# Bandit Level 3 → Level 4

## Level Goal

[url](https://overthewire.org/wargames/bandit/bandit4.html)

The password for the next level is stored in a hidden file in the **inhere** directory.

## Solution

```
$ cd inhere/ && ls -la
$ cat .hidden
# Copy password
$ ssh bandit4@bandit.labs.overthewire.org -p 2220
# type password
```

## Flag

`pIwrPrtPN36QITSp3EQaw936yaFoFgAB`