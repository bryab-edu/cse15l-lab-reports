# Lab Report 1 - Remote Access and FileSystem
## Using the `cd` command
No arguments - Within `/home/lecture1/` directory, goes to previous directory `\home\`. Not an error.
```
[user@sahara ~/lecture1]$ cd
[user@sahara ~]$ 
```
_directory_ as an argument - changes directory from `/home/` to the current argument `/home/lecture1/`. Not an error.
```
[user@sahara ~]$ cd lecture1
[user@sahara ~/lecture1]$
```
`file` as an argument - error, command asks for a directory as an argument. Even in `/lecture1/messages/` where the file _en-us.txt_ is present, the command outputs an error 
```
[user@sahara ~/lecture1/messages]$ cd en-us.txt
bash: cd: en-us.txt: Not a directory
```
## Using the `ls` command
No arguments - Displays all the files and directories from the current directory `/lecture1/messages/`. In this case, 3 text files. Not an error.
```
[user@sahara ~/lecture1/messages]$ ls
en-us.txt  es-mx.txt  zh-cn.txt
```
`directory` as an argument - Displays all the files and directories from the directory as inputted by the argument `/lecture1/`, since `/lecture1/` is in the current directory `/home/`, not an error.
```
[user@sahara ~]$ ls lecture1
Hello.class  Hello.java  messages  README
```
`file` as an argument - In the `/home/` directory, using the `ru.txt` file as the argument outputs the same file name `ru.txt`, not an error.
```
[user@sahara ~]$ ls ru.txt
ru.txt
```
## Using the `cat` command
No arguments - Leaves a blank space for the user to input text in which the command outputs the same text, this goes on until the user input **CTRL+C** to stop the command. Not an error. In `/home/` directory, not an argument
```
[user@sahara ~]$ cat
cat
cat
cat
cat
^C
[user@sahara ~]$
```
`directory` as an argument - Error, In `/home/` command states that the argument `/home/lecture1/` is a directory. Commands asks for file input. 
```
[user@sahara ~]$ cat lecture1
cat: lecture1: Is a directory
```
`file` as an argument - In `/home/`, outputs the file contents within the file input `ru.txt`. 
```
[user@sahara ~]$ cat ru.txt
Привет
```
