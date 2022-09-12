# Command Line Intro With Linux

### TL;DR

#### Essential file movement:

`man`, `ls`, `pwd`, `touch`, `rm`, `mkdir`, `rmdir`, `cd`, `cp`, `mv`

#### Essential Knowledge: 

flags change the behaviour of the command so read through the `man` pages to find out what is possible and what the result will be
the most important flag is `-h` or `--help`, these will print the help pages which are more concise than the man pages but at the same time more limited

## Introduction

There are a few essential commands to learn to get started with a unix operating system
These are default shell commands which should be a good foundation to begin to use the terminal more, obviously this is not an extensive list but should allow you to find further resources

### flags

flags are preceded by a dash and modify the functionality of the program so for example `ls -a` is just `ls` with the `-a` flag

### man

`man` are the linux man pages and takes a program name as an argument and gives detailed documentation of how exactly each available flag will modify the programs functionality
for example:
we can run the following command `man ls` to list the flags available to the ls command, in here we will find a lot of modifiers that could make our lives easier such as the `-a` flag which will print hidden directories as well as the standard ones, we could also use the `--color` flag which will colorize the output allowing us to easily differentiate between directories and different file extensions

<p align="center">
  <img alt-text="man command" src="/posts/assets/man_command" height="1500px" width="700px">
</p>

### ls

`ls` simply translates to list directory contents, there are multiple flags for ls which make it more capable, from the screenshot of the ls man page you can see that there is a lot that can be edited and a lot of flags available
This command is very basic but forms the backbone of many peoples daily workflow to know where they are in the computer and whats around you

![ls command](/posts/assets/ls_command)

### pwd

Now that we know what is around us, we need to know where we are to do that we can use`pwd` if the shell prompt doesn't let you know your location already. `pwd` takes no arguments and simply prints the current path and exits

<p align="center">
  <img alt-text="pwd command" src="/posts/assets/pwd_command" height="150px">
</p>

### touch

`touch` creates an empty file with the name as an argument and can also take a relative path  
*N.B.* an error will be thrown unless the directory exists that you are trying to create the file in

### rm 

`rm` removes a file by passing the file name or path as an argument, it can also remove a directory by passing the `-r` flag before specifying the path or directory name but it is usually used to delete single files  
*N.B.* Be aware of the power of `rm -rf /` as this will recursively delete every file on your computer although it may need super user priveleges `sudo`

<p align="center">
  <img alt-text="file command" src="/posts/assets/file_command" height="500px" width="300px">
</p>

### sudo

`sudo` can precede most commands on this list and gives you access to the system as the root user  temporarily, you may have to use root priveleges when installing packages from your distro package repository

~~no image here~~

### mkdir

`mkdir` means make directory and it does exactly that so you can create a directory in the current file or you can pass a relative path to the command.

### rmdir

`rmdir` is the opposite of mkdir and can only remove empty directories so to remove a directory and its contents we use `rm` with the `-r` flag, which stands for recursive

![mkdir and rmdir commands](/posts/assets/dir_command)

### cd

`cd` means change directory and allows us to move around changing our current working directory. The most useful commands with `cd` are `cd ..` which moves to a higher directory otherwise you can `cd` into a directory below

![cd command](/posts/assets/cd_command)

### cp

This is the terminal version of copy and all you have to do is pass the source and destination file to the program, i.e. `cp <source> <destination>`, this will copy the source file to the destination file

![cp command](/posts/assets/cp_command)

### mv

`mv` is similar to `cp` but it moves the source file to the destination location, it could also be considered a renaming tool because renaming is equivalent to moving to a new name

![mv command](/posts/assets/mv_command)

## Conclusion

These are some basic shell commands but with them you will be able to move around your terminal as well as start to build on top of them, the most important thing to remember is that there are `man` pages available with extensive documentation as well as the help flag which will sumarize everything

Thanks for reading and good luck in your future endeavours



