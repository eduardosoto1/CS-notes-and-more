# Introduction to Linux

# Table of Contents
- [What is Linux?](#what-is-linux)
- [Basic terminology](#basic-terminology)
- [The Terminal](#the-terminal)
- [Flags and Switches](#intro-to-flags-and-switches)
- [Filesystem Interaction](#filesystem-interaction)

# What is Linux

# Basic Terminology
- ls
    - ls -lh is used to list permissions of all files in the directory
    - Use the man tool to view what each letter does
    - The three columns can represent
        - Read
        - Write
        - Execute
```cpp
root@linux:~$ ls -lh
-rw-r--r-- 1 cmnatic cmnatic 0 Feb 19 10:37 file1
-rw-r--r-- 8 cmnatic cmnatic 0 Feb 19 10:37 file2
```
## Manual Page
• Advancing your use of commands by providing flags, switches and where you can go to learn about these for each command (man pages)


# The Terminal 
• How to connect to a Linux machine remotely using SSH


# Intro to Flags and Switches

# Filesystem Interaction

### Permissions

- To switch between users use the **su** command
    - This switches you to the root user
    - Requires passsword
- The -l or —login command
    - Starts shell similar to user logging into system

## Intro to Directories

- /etc
    - This root directory is used to store system files that are used by operating systems
- /var
    - Is short for variable data. It is a root folder found on a Linux install.
    - This folder stores data for applications or software running on the system.
    - Log files are commonly found here
- /root
    - The /root folder is actually the home for the “root” system user.
    - Understand that this is the home directory for “root” user and not related to /home
- /tmp
    - This is short for temporary.
    - The tmp directory is used to store data that wont be accessed a lot.
        - Whenever you turn off or restart your computer, the contents will be cleared out.

## Introduction to Terminal Text Editors

- Nano and VIM are the most popular forms of text editors
    - nano [NAME OF FILE]- replace “NAME OF FILE” with file of name you want to edit
    - The shortcuts could be seen in the terminal
- To navigate in Nano use the arrow keys or to start a new line “Enter” on the keyboard.
- Nano allows for easy features for you to remember
    - Use “ctrl” on keyboard with letter to access. (symbol is ^)
    - Searching for text (^W)
    - Copying and Pasting
    - Jumping to a line number
    - Finding out which line number you’re on.(^C)
- To exit Nano use (^X)
- Check out my page on VIM to learn VIM

## Daily Tasks

### Downloading files (wget)

- If you need files like a script, program, or images. There are multiple ways to retrieve files such as wget and curl(in another section)…
    - wget allows for downloading files through the network.
    - To use it just use:
    
    `wget [NAME OF HTTPS LINK]`
    

### Transferring files from Host - SCP (SSH)

- SCP or secure copy allows you to securely copy files
    - Copy files and directories from system to a remote system
    - Copy files & directories from a remote system to your system

        `scp important.txt ubuntu@192.168.1.30:/home/ubuntu/transferred.txt`

### Serving files from Host - WEB

- Python has a module called HTTPServer which makes your computer a web server that you can use to server files and downloaded by curl or wget.
- Python3’s “HTTPServer” will start a web server

`python3 -m http.server` 

### Challenge

Set up a http server in your home directory. Download a file to your host. 

# Introduction to Processes

- Processes are the programs that are running on machine
    - To view them use the **ps** command
    - Will display status code (PID), Sessiopn that is running it (TTY), How much usage time of the CPU it is using (TIME), CMD is name of actual command being executed or program.