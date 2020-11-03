# Bash Commands for Developers

Bash is a text-based interface that developers use to interact with an operating system. It is the default shell in Linux. Like all shells, bash acts as an interpreter whereby a user can implement commands to perform a wide variety of tasks. These tasks include managing data streams, manipulating files and directories, interacting with text files, and managing network services. A user can combine multiple bash commands in one script to perform complex operations.

Before you can use bash you must know which commands are available to you and what their functions are. You can view available commands by typing ```ls /bin ``` into the shell. The following are some common bash commands you may find useful.

## Navigating a Directory

### pwd

Identifies the current directory.

### cd

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

### ~

Represents the home directory of the current user.

For the root user, this will be /root.

### ls

List files in current directory.
```
ls
```

You can use switches to be more specific:

List all. Reveals all hidden files.
```
ls -a
```

Sort by most recently modified.
```
ls -t
```

## Manipulating Files and Directories

### mkdir
Make a directory. Takes directory name as argument.
```
mkdir directory-name
```

### rmdir
Remove a directory. This command only works if the directory is empty.
```
rmdir
```

### rm
Remove. Use for files and non-empty directories. Use great caution when using this command. The files you remove will not be recoverable. Take care to avoid typos.
```
rm filename
```

To remove all files in a directory, use the ```-r``` (recursive) switch.
```
rm -r directory-name
```

### touch
Creates a file. Can also use it to change the last-modification time of a file that already exists.
```
touch filename
```

### cp
Copy one file to another. Overwrites the receiving file.
```
cp file1 file2
```

### mv
Renames a file. Everything else about the file remains the same.
```
mv oldname newname
```

### ln
Link. Creating a linked file allows users to refer to the same file using a different name.
```
ln filename newname
```

### find
Search directories and subdirectories for a desired file.
```
find /path searchterm actiontoperform
```

Find is a complex and useful command that can take a wide variety of arguments not covered here.

### alias
Rename or simplify name of another command.

For this example, we'll create an alias for the ```ls``` command so that it returns hidden files without having to use the ```-a``` switch.
```
alias ls='ls -a'
```

## Manipulating Text Streams

A text stream is the movement of data. For example, the command ```cat filename``` streams the data from ```filename``` to the terminal.

### cat
Read a file.
```
cat filename
```
You can concatenate two files into a single output.
```
cat file1 file2
```

### more
A utility also known as a "pager" that lets you scroll through the text of a file from start to finish.
```
more /var/log/messages
```

### less
A utility known as a "pager" that lets you scroll through the text of a file using the arrow keys.
```
less /var/log/messages
```




