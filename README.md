## Bash Commands for Developers

Bash is a text-based interface that developers use to interact with an operating system. It is the default shell in Linux. Like all shells, bash acts as an interpreter whereby a user can implement commands to perform a wide variety of tasks. These tasks include managing data streams, manipulating files and directories, interacting with text files, and managing network services. A user can combine multiple bash commands in one script to perform complex operations.

Before you can use bash you must know which commands are available to you and what their functions are. You can view available commands by typing ls /bin into the shell. The following are a list of common bash commands you may find useful.

### Commands for Navigating a Directory

#### pwd

Identifies the current directory.

#### cd

Change directory. 

Used by itself, it takes you to the home directory.
```
cd
```

Use an argument containing an absolute path to a directory to move there.
```
cd ~/projects/projectname
```

Two periods as an argument take you back one directory.
```
cd ..
```

Use slashes to move back multiple levels of directory.
```
cd ../../..
```

#### ~

Represents the home directory of the current user.

For the root user, this will be /root.

#### ls

List files in current directory. You can use switches to be more specific.
```
ls -a
```
List all. Reveals all hidden files.

```
ls -r
```
Reverse listing order.




