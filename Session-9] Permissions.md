# Permissions in Linux-
- Linux File System Security restricts user to access the files and directories.
- User require permissions to access files or directories.
- “ls -l” or “ll” command can be used to check security of any file or directory.
- Above command will display contents from directory along with its security 
details.
### drwxr-xr-x 3 root root     4096 May  9 18:41 Linux
### -rw-rw-r-- 1 root root 60582753 May 10 12:02 file1.txt
* The first character = ‘-‘, which means it’s a file ‘d’, which means it’s a directory.
* The next nine characters = (rw-r–r–) show the security
* The next column shows the owner of the file. (Here it is `root`)
* The next column shows the group owner of the file. (Here it is `root` which has special access to these files)
* The next column shows the size of the file in bytes.
* The next column shows the date and time the file was last modified.
* Last Column = File_name or Directory_name. (For example, here are: prac, snap, test, example)
# Types of file-
## Ordinary File/ Regular File- (start with _)
- File which contain Data. 
- Regular files are nothing but the everyday files used to store information such as text, or images.
- These files can be found in directories, which are yet another type of files. 
- In Linux, regular files can exist with or without an extension.
## Directory File- (Start with d)
- Directory file is equal to folder, it contains files and folders.
- Directories are also Linux files. But rather than storing data, they store the location of other files. To achieve this, the directory uses directory entries. 
## Link File- 
- A link is a symbolic connection or pointer to a single file that allows you to access it from more than one directory.
- You can set up a link to a file in a restricted directory, allowing access to the file without providing access to the directory.
- Soft link- Link will be removed if original file removed. A hard link develops a mirror copy of the original file.
#### Synatx to create softlink,
* ln –s <original_file> <softlink_name>
- Hard link- Renaming, deleting or removing file will not effect link. soft or symbolic link creates a pointer to the original file.
#### Syntax to create hardlink,
* ln <original_file> <hardlink_name>
## Named Pipe file- (start with p)  
- used to establish two-way communications between two unrelated programs.
- Sends data from one process to another so that receiving process reads the data FIFO manner.
- These files are present in /run folder.
## Socket file- (start with s)
- Special file to enable communications between two processes.
- These files are present in /run folder.
## Character file-  (start with c)
- Reads and write data character by character.
- These files are present in /dev folder.
- A character device file is a hardware file that reads or writes data one character at a time in a file.
## Block Device file- (start with b)
- file that refers to device. 
- a piece of hardware that provides data access in blocks
# Three types of permissions-
### Read (r): 
- Allows reading and viewing the contents of a file or directory.
### Write (w): 
- Grants the ability to modify, delete, or add to the contents of a file or directory.
### Execute (x):
- Enables the execution of a file or allows access to a directory's contents if used with directory permissions.

# These permissions are set for four categories of users:
### Owner: (u)
- The user who owns the file or directory.
### Group: (g)
- Users who are members of the group associated with the file or directory.
### Others: (o)
- All other users who are not the owner or part of the group.
### All: (a)

# Permissions are represented by a series of symbols:
* r: indicates read permission.
* w: indicates write permission.
* x: indicates execute permission.
* -: indicates no permission.

# Symbols:  

* `+`	Add permissions
* `-`	Remove permissions
* `=`	Set the permissions to the specified values


