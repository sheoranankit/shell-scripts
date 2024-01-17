The kernel is the heart of the Linux operating system. It manages the resources of Linux such as:

  File management
  Multitasking
  Memory management
  I/O management
  Process management
  Device management
  Networking support including IPv4 and IPv6
Advanced features such as virtual memory, shared libraries, demand loading, shared copy-on-write executables etc
The kernel decides who will use these resources and for how long and when. It runs your programs or sets up to execute binary files. The kernel acts as an intermediary between the computer hardware and various applications.


![image](https://github.com/sheoranankit/shell-scripts/assets/56736557/746e74b9-82e1-44fc-89a0-3ee9b8bad7a9)


cat /etc/shells

# List of acceptable shells for chpass(1).
# Ftpd will not allow users to connect who are not using
# one of these shells.

/bin/bash
/bin/csh
/bin/dash
/bin/ksh
/bin/sh
/bin/tcsh
/bin/zsh

Basic Command Line Editing
You can use the following key combinations to edit and recall commands:

CTRL + L : Clear the screen.
CTRL + W : Delete the word starting at cursor.
CTRL + U : Clear the line i.e. Delete all words from command line.
Up and Down arrow keys : Recall commands (see command history).
Tab : Auto-complete files, directory, command names and much more.
CTRL + R : Search through previously used commands (see command history)
CTRL + C : Cancel currently running commands.
CTRL + T : Swap the last two characters before the cursor.
ESC + T : Swap the last two words before the cursor.
CTRL + H : Delete the letter starting at cursor.

**Each shell script consists of
**Shell keywords such as if..else, do..while.
Shell commands such as pwd, test, echo, continue, type.
Linux binary commands such as w, who, free etc..
Text processing utilities such as grep, awk, cut.
Functions - add frequent actions together via functions. For example, /etc/init.d/functions file contains functions to be used by most or all system shell scripts in the /etc/init.d directory.
Control flow statments such as if..then..else or shell loops to perform repeated actions.
Each script has purpose
Specific purpose - For example, backup file system and database to NAS server.
Act like a command - Each shell script is executed like any other command under Linux.
Script code usability - Shell scripts can be extended from existing scripts. Also, you can use functions files to package frequently used tasks.
