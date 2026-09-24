### Level Goal
The password for the next level is stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions
## access server with password exist in level-10_11.md
ssh bandit11@bandit.labs.overthewire.org -p 2220

## execute this command to see the password

```
awk -F ' ' '{print $4}' data.txt  | tr 'N-ZA-Mn-za-m' 'A-Za-z' && printf "\n"
```

## password is 

```
GROozWPO8QyN0mGrjUkID0WCYkZiQxrN
```

