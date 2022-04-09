# Week 2 Lab Report (1)
### Introduction
On this page, you will be guided step-by-step on how to remotely access your ieng account on your local device. The steps are as follows:
1. Installing VScode
2. Remotely Connecting
3. Trying Some Commands
4. Moving Files with scp
5. Setting an SSH Key
6. Optimizing Remote Running

### 1. Installing Visual Studio Code (VSCode)
The first step is to visit the [official VSCode website](https://code.visualstudio.com/) and download VSCode onto your device.
Click the "Download" button for your operating system.

After downloading, make sure that it opens to a page similar to the one below.
![](image1.png)
### 2. Remotely Connecting
Windows users have a prestep: which is to download [OpenSSH](https://docs.microsoft.com/en-us/windows-server/administration/openssh/.openssh_install_firstuse).

Students will have to look up their account on the [SDACS](https://sdacs.ucsd.edu/~icc/index.php) site.

On VSCode, open up a terminal and type the following command, replacing zz with your specific id.

`$ ssh cs15lsp22zz@ieng6.ucsd.edu`

If it is your first time connecting, you will receive a message asking if you want to connect. Say yes, and then it will prompt you to put in your password. Afterwards, you should be logged into the server remotely.
### Trying Some Commands
Here are some commands to try. Make sure to test them both on your local device as well as while connected to the server.
```
* cd ~
* cd
* ls -lat
* ls -a
* ls <directory> where <directory> is /home/linux/ieng6/cs15lsp22/cs15lsp22abc, where the abc is one of the other group members’ username
* cp /home/linux/ieng6/cs15lsp22/public/hello.txt ~/
* cat /home/linux/ieng6/cs15lsp22/public/hello.txt
(Copied directly from the Lab 1)
```
To exit, use the "exit" command.
### Moving files with scp
