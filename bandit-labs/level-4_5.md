### Level Goal
The password for the next level is stored in the only human-readable file in the inhere directory
## access server with password exist in level-3_4.md
ssh bandit4@bandit.labs.overthewire.org -p 2220

## execute this command to see the password

```
find inhere/ -type f |xargs file -i | grep -i ascii
cat inhere/-file07
```

## password is 

```
6C7h9GD8M6ai5nr7wo1RonrzFjj9yIrG
```

