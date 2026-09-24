### Level Goal
The password for the next level is stored in the file data.txt and is the only line of text that occurs only once
## access server with password exist in level-7_8.md
ssh bandit8@bandit.labs.overthewire.org -p 2220

## execute this command to see the password

```
sort data.txt | uniq -u 
```

## password is 

```
EjmOSvuAu7sGAHqHVcBDPirRe9T03kxl
```

