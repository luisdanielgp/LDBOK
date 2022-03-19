# Bandit Level 2 → Level 3

## Level Goal

[url](https://overthewire.org/wargames/bandit/bandit3.html)

The password for the next level is stored in a file called **spaces in this filename** located in the home directory

## Solution

```
$ cat spaces\ in\ this\ filename
# Copy password
$ ssh bandit3@bandit.labs.overthewire.org -p 2220
# type password
```

## Flag

`UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK`