# Bandit Level 4 → Level 5

## Level Goal

[url](https://overthewire.org/wargames/bandit/bandit5.html)

The password for the next level is stored in the only human-readable file in the **inhere** directory. Tip: if your terminal is messed up, try the “reset” command.

## Solution

```
$ file inhere/*
inhere/-file00: data
inhere/-file01: data
inhere/-file02: data
inhere/-file03: data
inhere/-file04: data
inhere/-file05: data
inhere/-file06: data
inhere/-file07: ASCII text
inhere/-file08: data
inhere/-file09: data

# cat ASCII text file
$ cat inhere/-file07
koReBOKuIDDepwhWk7jZC0RTdopnAYKh

# Copy password
$ ssh bandit5@bandit.labs.overthewire.org -p 2220
# type password
```

## Flag

`koReBOKuIDDepwhWk7jZC0RTdopnAYKh`