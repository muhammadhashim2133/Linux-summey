# Linux Summary

## Introduction to Operating Systems (OS)
An operating system is a program that serves as an interface between a computer's user and its hardware.

## Why Linux?
- Free and open source
- Stability and reliability
- Security
- Flexibility: Customizable to user needs

## What is Linux?
Linux is an open source operating system.

## Kernel
The kernel facilitates communication between hardware and applications, acting as a bridge between them.

## Kernel & User Space
The system's main memory is divided into two sections: kernel space and user space. User space contains multiple programs, requiring kernel space for their execution. 
- Kernel space is accessible to user processes solely through system calls.
- Linux employs standard libraries for system calls, such as the GNU C Library, which provides functions like printing and writing.

## File System
- Linux organizes files hierarchically.
- Files are stored in directories, which can also contain other directories.
- Unlike Windows, Linux does not use drive letters.

## Linux Commands
- `cd /`: Move to the root directory.
- `ls`: List the contents of the current directory.
- `cd home/`: Change to the "home" directory.
- `~`: Represents the user's home directory.
- `cd ..`: Move up one directory level.
- `mkdir directoryname`: Create a directory with the given name.
- `touch app.txt`: Create a file named "app.txt".
- `vi app.txt`: Use the vi editor to edit files. Press 'i' to enter insert mode, write your text, press 'Esc' to exit insert mode. To save, press 'Shift' + ':' and then enter 'wq' (write and quit).
- `cat app.txt`: Display the contents of "app.txt".
- `cp app.txt /home/hashim/desktop/cloud-native`: Copy "app.txt" to the "cloud-native" directory.
- `mv app.txt /home/hashim/desktop`: Move "app.txt" to the desktop.
- `rm /home/hashim/desktop/app.txt`: Remove "app.txt" from the desktop.
- `find /home/hashim/desktop/cloud-native/ -name "app.txt"`: Search for the file or directory "app.txt" in the specified path.
- `man mkdir`: Show details about the "mkdir" command.
- `uname`: Display the operating system name.
- `uname -a`: Display detailed machine information, including processor architecture and OS details.
- `ls cpu`: Return information about the system, CPU speed, and count.
- `df -h`: Display disk space in human-readable format.
- `du home/daniyal/desktop/cloud-native/cli`: Display the size of the specified directory.
- `du -s /home/daniyal/desktop/cloud-native/cli`: Display the total space used by the specified directory.
- `date`: Display the current date.
- `cal`: Display the calendar.
- `w`: Show who is online.
- `apt-get install package-name`: Install a specific package.
- `apt-cache search keyword`: Search for packages related to the keyword.
- `info`: Provide information about commands.
- `type man`: Show the location of the command's manual file.
- `pg`: Display background services.
- `free`: Show available memory.
- `ps`: Show running services.
- `kill processid`: Terminate a process.
- `nice`: Run a program with low priority.
- `top`: Display running processes.
- `su -`: Switch to the root user in the shell.
- `shutdown`: Turn off the computer.
## User Roles, SUDO, Command Completion, History, Scripting, File Permissions, and General Commands

## User Roles and SUDO

- `sudo su`: Logs in as the root user, allowing you to install packages using commands like `apt-get install python`.

- `sudo apt-get install python`: With sudo, you can install packages without needing to switch to the root user.

## Command Completion and History

- To auto-complete a command, type the first few letters of the command and press `Tab` to complete it.

- Use `Ctrl + A` to move the cursor to the beginning of the line and `Ctrl + E` to move the cursor to the end.

## Scripting

Scripts are used for repetitive tasks.
- Create a new shell script file: `touch simple.sh`
- Edit the script file: `vi simple.sh`
- Press `i` to enter insert mode.
- Write the first lines:
  ```bash
  #!/bin/bash
  echo "My first name is: $1"
  echo "My last name is: $2"


## File Permissions
In Linux and Unix-like operating systems, file permissions determine access rights for files and directories. Each permission is represented by a numeric value:

- 0: No permission
- 1: Executable permission
- 2: Write permission
- 4: Read permission

You can check permissions using the `ls -l` command and modify them using `chmod`.
ls -l
chmod 777 simple.sh
./simple.sh hashim shabbir

## General Commands

- `uptime`: Displays the amount of time your system has been up.
- `uname`: Shows information about the operating system.
- `uname -srv`: Displays the operating system name, version, and release.
- `man ls`: Displays comprehensive details about the mentioned command.
- `pwd`: Shows the path of the current working directory.
- `hostname`: Displays the hostname of the system.
- `hostname -i`: Displays the IP address of the system.

## Create Custom Commands
`alias myfile="rouch myfile.txt` is a custome command that create myfile.txt





