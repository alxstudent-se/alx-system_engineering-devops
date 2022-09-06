# Shell Basics

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://github.com/alxstudent-se/alx-system_engineering-devops.git)



#### 0-current_working_directory
>Write a script that prints the absolute path name of the current working directory.
```sh
#!/bin/bash
pwd
```


#### 1-listit
>Display the contents list of your current directory.
```sh
#!/bin/bash
ls
```
#### 2-bring_me_home
>Write a script that changes the working directory to the user’s home directory.

```sh
#!/bin/bash
cd ~
```
#### 3-listfiles
>Display current directory contents in a long format

```sh
#!/bin/bash
ls -l
```
#### 4-listmorefiles
>Display current directory contents, including hidden files (starting with .). Use the long format.

```sh
#!/bin/bash
ls -la
```
#### 5-listfilesdigitonly
>Display current directory contents.

```sh
#!/bin/bash
ls -la
```
#### 6-firstdirectory
>Create a script that creates a directory named my_first_directory in the /tmp/ directory.

```sh
#!/bin/bash
mkdir /tmp/my_first_directory
```
#### 7-movethatfile
>Move the file betty from /tmp/ to /tmp/my_first_directory.

```sh
#!/bin/bash
mv /tmp/betty /tmp/my_first_directory
```
#### 8-firstdelete
>Delete the file betty.
The file betty is in /tmp/my_first_directory

```sh
#!/bin/bash
rm /tmp/my_first_directory/betty
```
#### 9-firstdirdeletion
>Delete the directory my_first_directory that is in the /tmp directory.

#!/bin/bash
```sh
rmdir /tmp/my_first_directory
```
#### 10-back
>Write a script that changes the working directory to the previous one.
10-back
```sh
#!/bin/bash
cd -
```
#### 11-lists
>Write a script that lists all files (even ones with names beginning with a period character, which are normally hidden) in the current directory and the parent of the working directory and the /boot directory (in this order), in long format.

```sh
#!/bin/bash
ls -la . .. /boot
```
#### 12-file_type
>Write a script that prints the type of the file named iamafile. The file iamafile will be in the /tmp directory when we will run your script.

```sh
#!/bin/bash
file /tmp/iamafile
```
#### 13-symbolic_link
>Create a symbolic link to /bin/ls, named __ls__. The symbolic link should be created in the current working directory.

```sh
#!/bin/bash
ln -s /bin/ls __ls__
```
#### 14-copy_html
>Create a script that copies all the HTML files from the current working directory to the parent of the working directory, but only copy files that did not exist in the parent of the working directory or were newer than the versions in the parent of the working directory.

```sh
#!/bin/bash
cp -n *.html ..
```
#### 100-lets_move
>Create a script that moves all files beginning with an uppercase letter to the directory /tmp/u.

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
#### 102-tree
>Create a script that creates the directories welcome/, welcome/to/ and welcome/to/school in the current directory.

```sh
#!/bin/bash
mkdir -p welcome/to/school
```
#### 103-commas
>Write a command that lists all the files and directories of the current directory, separated by commas (,).

```sh
#!/bin/bash
ls -map|sort -d
```
#### school.mgc
>Create a magic file school.mgc that can be used with the command file to detect School data files. School data files always contain the string SCHOOL at offset 0
```sh
Ò
```

   