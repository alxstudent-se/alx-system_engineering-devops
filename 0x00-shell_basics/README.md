0-current_working_directory
```sh
#!/bin/bash
pwd
```


1-listit
```sh
#!/bin/bash
ls
```

>Write a script that changes the working directory to the user’s home directory.
>2-bring_me_home
```sh
#!/bin/bash
cd ~
```

>Display current directory contents in a long format
3-listfiles
```sh
#!/bin/bash
ls -l
```

>Display current directory contents, including hidden files (starting with .). Use the long format.
4-listmorefiles
```sh
#!/bin/bash
ls -la
```
>Display current directory contents.
5-listfilesdigitonly
```sh
#!/bin/bash
ls -la
```
>Create a script that creates a directory named my_first_directory in the /tmp/ directory.
6-firstdirectory
```sh
#!/bin/bash
mkdir /tmp/my_first_directory
```
>Move the file betty from /tmp/ to /tmp/my_first_directory.
7-movethatfile
```sh
#!/bin/bash
mv /tmp/betty /tmp/my_first_directory
```
>Delete the file betty.
The file betty is in /tmp/my_first_directory
8-firstdelete
```sh
#!/bin/bash
rm /tmp/my_first_directory/betty
```
>Delete the directory my_first_directory that is in the /tmp directory.
9-firstdirdeletion
#!/bin/bash
```sh
rmdir /tmp/my_first_directory
```
>Write a script that changes the working directory to the previous one.
10-back
```sh
#!/bin/bash
cd -
```
>Write a script that lists all files (even ones with names beginning with a period character, which are normally hidden) in the current directory and the parent of the working directory and the /boot directory (in this order), in long format.
11-lists
```sh
#!/bin/bash
ls -la . .. /boot
```
>Write a script that prints the type of the file named iamafile. The file iamafile will be in the /tmp directory when we will run your script.
12-file_type
```sh
#!/bin/bash
file /tmp/iamafile
```
>Create a symbolic link to /bin/ls, named __ls__. The symbolic link should be created in the current working directory.
13-symbolic_link
```sh
#!/bin/bash
ln -s /bin/ls __ls__
```
>Create a script that copies all the HTML files from the current working directory to the parent of the working directory, but only copy files that did not exist in the parent of the working directory or were newer than the versions in the parent of the working directory.
14-copy_html
```sh
#!/bin/bash
cp -n *.html ..
```
>Create a script that moves all files beginning with an uppercase letter to the directory /tmp/u.
100-lets_move
```sh
#!/bin/bash
mv [[:upper:]]* /tmp/u
```
>Create a script that deletes all files in the current working directory that end with the character ~.
101-clean_emacs
```sh
#!/bin/bash
rm *~
```
>Create a script that creates the directories welcome/, welcome/to/ and welcome/to/school in the current directory.
102-tree
```sh
#!/bin/bash
mkdir -p welcome/to/school
```
>Write a command that lists all the files and directories of the current directory, separated by commas (,).
103-commas
```sh
#!/bin/bash
ls -map|sort -d
```
```sh
school.mgc
Ò
```
