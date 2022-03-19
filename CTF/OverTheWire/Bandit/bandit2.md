# Bandit Level 1 → Level 2

## Level Goal

[url](https://overthewire.org/wargames/bandit/bandit2.html)

The password for the next level is stored in a file called **-** located in the home directory

## Solution

```
$ cat < -
# Copy password
$ ssh bandit2@bandit.labs.overthewire.org -p 2220
# type password
```

## Flag

`CV1DtqXWVFXTvM2F0k09SHz0YwRINYA9`