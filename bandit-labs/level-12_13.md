### Level Goal
The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work. Use mkdir with a hard to guess directory name. Or better, use the command “mktemp -d”. Then copy the datafile using cp, and rename it using mv (read the manpages!)
## access server with password exist in level-11_12.md
ssh bandit12@bandit.labs.overthewire.org -p 2220

## execute this command to see the password

```

xxd -r data.txt output1  ==> hexdump to original file
file -b output1  ==> type gz
mv output1 output1.gz ==>  add extension for decompression 
gzip -d output1.gz ==> decompress
file -b output1  ==> type bz2
mv output1 output1.bz2 ==> add extension
bzip2 -d output1.bz2
file -b output1  ==> type gz
mv output1 output1.gz ==> add extension 
gzip -d output1.gz ==> decompress
file -b output1   ==> type tar 
mv output1 output1.tar.gz
tar -xvf output1.tar.gz  ==> extract 
file -b data5.bin  ==> tar file 
mv data5.bin data5.tar.gz
file -b data6.bin  ==> type bz2
mv data6.bin data6.bz2
file -b data6 ==> tar file
mv data6 data6.tar.gz
tar -xvf data6.tar.gz 
file -b data8.bin ==> gz file
mv data8.bin data8.gz
gzip -d data8.gz  
file -b data8 ==> ascci file 
 ==> cat data8  ==> password found 
```

## password is 

```
qQYQiHOBPR8zR61qxYqX45quvihF2uzk
```

