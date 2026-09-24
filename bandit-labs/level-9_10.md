### Level Goal
The password for the next level is stored in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.
## access server with password exist in level-8_9.md
ssh bandit9@bandit.labs.overthewire.org -p 2220

## execute this command to see the password

```
strings data.txt | grep -E "={2,}.*" 
```

## password is 

```
B0s2khmbT9u0geKuOoVGW3JZKhndE3BG
```

