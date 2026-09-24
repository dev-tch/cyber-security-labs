### Level Goal
The password for the next level is stored somewhere on the server and has all of the following properties:

owned by user bandit7
owned by group bandit6
33 bytes in size
## access server with password exist in level-5_6.md
ssh bandit6@bandit.labs.overthewire.org -p 2220

## execute this command to see the password

```
find / -type f -user bandit7 -group bandit6 -size 33c 2> /dev/null
cat /var/lib/dpkg/info/bandit7.password
```

## password is 

```
Bmnnvf82KzQlfxgAI2d1zYbr1u9pr3E3
```

