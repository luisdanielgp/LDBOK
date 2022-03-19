# Bandit Level 6 → Level 7

[url](https://overthewire.org/wargames/bandit/bandit7.html)

## Level Goal

The password for the next level is stored **somewhere on the server** and has all of the following properties:

-   owned by user bandit7
-   owned by group bandit6
-   33 bytes in size

```
$ cd ../..
$ find . -user bandit7 -group bandit6 -size -2 -exec ls -la -S -s {} \;
...
4 -rw-r----- 1 bandit7 bandit6 33 May  7  2020 ./var/lib/dpkg/info/bandit7.password
...
$ cat ./var/lib/dpkg/info/bandit7.password
HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs
$ ssh bandit7@bandit.labs.overthewire.org -p 2220
# type password
```

## Flag

`HKBPTKQnIay4Fw76bEy8PVxKEDQRKTzs`

## Resources
+ [Use the Unix find command to search for files](https://kb.iu.edu/d/admm)