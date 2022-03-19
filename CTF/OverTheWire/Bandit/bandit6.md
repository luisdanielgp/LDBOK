# Bandit Level 5 → Level 6

[url](https://overthewire.org/wargames/bandit/bandit6.html)

## Level Goal

The password for the next level is stored in a file somewhere under the **inhere** directory and has all of the following properties:

-   human-readable
-   1033 bytes in size
-   not executable

```
$ find inhere/ \( -size +2 -size -4 \) -exec ls -la {} \;
...
-rw-r----- 1 root bandit5 1033 May  7  2020 inhere/maybehere07/.file2
...

$ cat inhere/maybehere07/.file2
DXjZPULLxYr17uwoI01bNLQbtFemEgo7
$ ssh bandit6@bandit.labs.overthewire.org -p 2220
# type password
```

## Flag

`DXjZPULLxYr17uwoI01bNLQbtFemEgo7`

## Resources
+ [Use the Unix find command to search for files](https://kb.iu.edu/d/admm)