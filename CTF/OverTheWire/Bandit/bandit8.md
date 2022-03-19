# Bandit Level 7 → Level 8

[url](https://overthewire.org/wargames/bandit/bandit8.html)

## Level Goal

The password for the next level is stored in the file **data.txt** next to the word **millionth**

```
$ grep "millionth" data.txt
millionth	cvX2JJa4CFALtqS87jk27qwqGhBM9plV
# close ssh connection
$ ssh bandit8@bandit.labs.overthewire.org -p 2220
# type password
```

## Flag

`cvX2JJa4CFALtqS87jk27qwqGhBM9plV`