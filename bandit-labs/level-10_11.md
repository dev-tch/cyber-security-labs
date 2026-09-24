### Level Goal
The password for the next level is stored in the file data.txt, which contains base64 encoded data
## access server with password exist in level-9_10.md
ssh bandit10@bandit.labs.overthewire.org -p 2220

## execute this command to see the password

```
cat data.txt | base64 -d 
```

## password is 

```
pYfOY6HwUsDj5rL9UvyhU7MCmv8vN5Ro
```

