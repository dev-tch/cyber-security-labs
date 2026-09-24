### Level Goal
The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

human-readable
1033 bytes in size
not executable
## access server with password exist in level-4_5.md
ssh bandit5@bandit.labs.overthewire.org -p 2220

## execute this command to see the password

```
find inhere/ -type f -size 1033c
cat inhere/maybehere07/.file2
```

## password is 

```
pXa26xhMWaC2SvDotA4r9EgZkulOeSBW
```

