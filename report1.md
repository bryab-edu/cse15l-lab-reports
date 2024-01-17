# Lab Report 1 - Remote Access and FileSystem
## Using the _cd_ command
No arguments - nothing happens, no directory to change towards. Thus commands does nothing, not an error, waiting for argument
```
[user@sahara ~]$ cd
[user@sahara ~]$ 
```
_directory_ as an argument - changes directory [from /home/] to the current argument [/home/lecture1/]
```
[user@sahara ~]$ cd lecture1
[user@sahara ~/lecture1]$
```
_file_ as an argument - error, command asks for a directory as an argument. Even in [/lecture1/messages/] where the file _en-us.txt_ is present, the command outputs an error 
```
[user@sahara ~/lecture1/messages]$ cd en-us.txt
bash: cd: en-us.txt: Not a directory
```
## using the _ls_ command
No arguments - Displays all the files and directories from the current directory [/lecture1/messages/]. In this case, 3 text files.
```
[user@sahara ~/lecture1/messages]$ ls
en-us.txt  es-mx.txt  zh-cn.txt
```
_directory_ as an argument - Displays all the files and directories from the directory as inputted by the argument [/lecture1/], since [/lecture1/] is in the current directory [/home/]
```
[user@sahara ~]$ ls lecture1
Hello.class  Hello.java  messages  README
```
