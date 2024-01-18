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




List of command bash keywords and built in commands
JOB_SPEC &
(( expression ))
. filename
[[:]]
[ arg... ]
expression
alias
bg
bind
builtin
caller
case
command
compgen
complete
continue
declare
dirs
disown
echo
enable
eval
exec
exit
export
false
fc
fg
for
getopts
hash
help
history
if
jobs
kill
let
local
logout
popd
printf
pushd
pwd
read
readonly
return
select
set
shift
shopt
source
suspend
test
time
times
trap
true
type
typeset
ulimit
umask
unalias
unset
until
variables
while


which command
You can also use the which command to display the full path of (shell) commands:

which commandname
which bash
Sample outputs:

/bin/bash
For each of its command line arguments it prints to stdout (screen) the full path of the executables that would have been executed when this argument had been entered at the shell prompt:

which date
which gcc
which vi
However, which cannot tell you exactly what the shell will execute in all cases as it is an external command. For more accurate information, use type command as follows:

type -p commandName
type -p bash
type -p date
type -p gcc
type -p echo

**Essential Vi Commands
Open a file:
vi filename
To go into edit mode:
press ESC and type I
To go into command mode:
press ESC
To save a file
press ESC and type :w fileName
To save a file and quit:
press ESC and type :wq
OR

press ESC and type :x
To jump to a line:
press ESC and type :the line number
To Search for a string:
Press ESC and type /wordToSearch
To quit vi:
Press ESC and type :q
Save the following into a file called hello.sh:

#!/bin/bash
echo "Hello, World!" 
echo "Knowledge is power."
Save and close the file. You can run the script as follows:

 ./hello.sh
