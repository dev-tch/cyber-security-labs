### Level Goal
The password for the next level is stored in /etc/bandit_pass/bandit14 and can only be read by user bandit14. For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level. Look at the commands that logged you into previous bandit levels, and find out how to use the key for this level.
If you need help with this level: a hint file can be found in the home directory.
Make sure to read the error messages as they are informative.
## access server with password exist in level-12_13.md
ssh bandit13@bandit.labs.overthewire.org -p 2220

## execute this command to see the password

```
scp -P 2220 bandit13@bandit.labs.overthewire.org:sshkey.private .
chmod 600 ./sshkey.private
ssh -i ./sshkey.private bandit14@bandit.labs.overthewire.org -p 2220
```

## password is 

```
aaWecNkG4FhxJQxz07uiwzVP6bJiYS65
```

