# WEEK 1 Lab Report

## Introduction
The goal of this week's lab is introducing Edstem and setting up a Workspace, which comes with the file system and a terminal to practice command lines and simple commands. During this week's labs, we practiced with cd, ls, and cat. Below are some of the commands we worked with.

## cd  


**Share an example of using the command with no arguments**
```
[user@sahara ~]$ cd lecture1/messages/
[user@sahara ~/lecture1/messages]$ cd
[user@sahara ~]$ pwd
/home
```
- using the cd command was run in the `messages` working directory
- the cd with no argument moves to `home`  directory from previous (`messages`) directory
- this is shown in the next line that we are in `home` directory because there are no other directory names
  
**Share an example of using the command with a path to a directory as an argument**
```
[user@sahara ~]$ cd lecture1
[user@sahara ~/lecture1]$ 
```
- working directory command was run in the `home` directory
- `cd` command changes the current directory to a specific directory given by the name listed next to the `cd` command
- The output on the next line was lecture1 next to the `~`, which means that `lecture1` became the working directory which is the correct output.

**Share an example of using the command with a path to a file as an argument**
```
[user@sahara ~/lecture1]$ cd lecture1/Hello.class
bash: cd: lecture1/Hello.class: No such file or directory
[user@sahara ~/lecture1]$ 
```
- working directory command was run in `home` directory
- this is output because `Hello.class` is not a directory so it cannot be accessed by `cd` command
- the output above is an error because we are not `Hello.class` directory, and did not output as intended
  

## ls 
**Share an example of using the command with no arguments**
```
[user@sahara ~/lecture1]$ ls
Hello.class  Hello.java  messages  README
[user@sahara ~/lecture1]$
```
- working directory: `lecture1` directory where `ls` command was run in
- `ls` command lists the content of the current working directory
- this output is correct since these are the files and directories within `lecture1` directory

**Share an example of using the command with a path to a directory as an argument**
```
[user@sahara ~]$ ls lecture1/messages/
en-us.txt  es-mx.txt  zh-cn.txt
[user@sahara ~]$ 
```
- `ls` command was run in `home` directory
- this output is shown because path written led to `messages` directory and listed content within `messages` directory
- it is the correct output because this is the right content in the `messages` directory

**Share an example of using the command with a path to a file as an argument**
```
[user@sahara ~]$ ls lecture1/messages/en-us.txt 
lecture1/messages/en-us.txt
[user@sahara ~]$ 
```
- working directory the command run in:  `home`
- `ls` command lists contents of a directory
- in this case it is used for a file
- the ouput is not an error since `ls` is working as intended to
  

## cat
**Share an example of using the command with no arguments**
```
[user@sahara ~]$ cat
im using this command with no arguments 
im using this command with no arguments 
i will type control d to end
i will type control d to end
[user@sahara ~]$ 
```
- working directory where command was run in: `home`
- when `cat` is used with no arguments it waits for input from user and displays what user inputs until user types `control D`
- output is correct until user types `control D`


**Share an example of using the command with a path to a directory as an argument**
```
[user@sahara ~]$ cat lecture1/messages/
cat: lecture1/messages/: Is a directory
[user@sahara ~]$ 
```
- working directory where command was run in: `home`
- output is shown because path was written to `messages` directory
- `cat` is used to access contents in a file
- output is an error because `cat` accesses the contetns in a file not in a directory such as `messages`

**Share an example of using the command with a path to a file as an argument**
```
[user@sahara ~]$ cat lecture1/README
To use this program:

javac Hello.java
java Hello messages/en-us.txt
```
- working directory where the command was run in: `home`
- `cat` command shows contents that are within file passed in the argument
- output is correct because the contents listed match the contents in the file when opened


</br>

</br>


# WEEK 3 LAB REPORT

## PART 1
**Writing a web server**

In part 1, I wrote a piece of code called ChatServer. The goal of ChatServer is to keep track of a single string that gets added to by incoming requests.





