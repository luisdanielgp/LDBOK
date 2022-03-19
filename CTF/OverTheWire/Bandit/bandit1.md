# Bandit Level 0 → Level 1

## Level Goal

[url](https://overthewire.org/wargames/bandit/bandit1.html)

The password for the next level is stored in a file called **readme** located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.

## Solution

```
$ cat readme
# copy password
# close ssh connection
$ ssh bandit1@bandit.labs.overthewire.org -p 2220
# type password
```

## Flag

`boJ9jbbUNNfktd78OOpsqOltutMc3MY1`