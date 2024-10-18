* The chown and chgrp commands used to change the ownership and group ownership of files and directories, respectively.

## chown (Change Ownership):
- The chown command changes the ownership of a file or directory.
- You can specify both the user (owner) and the group to which the file or directory will belong.

#### Syntax:
chown user :group file/dir
- chown newowner file.txt
- chown newowner :newgroup directory/filename

## chgrp (Change Group):
- The chgrp command changes the group ownership of a file or directory.
- You can specify only the group to which the file or directory will belong.

#### Syntax:
chgrp group file/dir
- chgrp newgroup file.txt


# How to Change Permissions in Linux-
- The command you use to change the security permissions on files is called “chmod“, which stands for “change mode".
### Syntax-
* chmod <u,g,o,a><+,-,=><r,w,x> <file_name>
# Octal Notation Method-
### Syntax- 
* chmod <permission_in_numbers> <file_name>

| Octal | Binary | Permission                |
|-------|--------|---------------------------|
| 0     | 000    | No permission (---)      |
| 1     | 001    | Execute (--x)             |
| 2     | 010    | Write (-w-)               |
| 3     | 011    | Write and execute (-wx)   |
| 4     | 100    | Read (r--)                |
| 5     | 101    | Read and execute (r-x)    |
| 6     | 110    | Read and write (rw-)      |
| 7     | 111    | Read, write, and execute (rwx) |


* chmod <permission_in_numbers> <file_name>
- chmod 644 example.txt

  
# Default Permissions (umask)-
- The umask command is used to set the default permissions mask for new files and directories. 
- It determines which permissions are removed or masked when a new file or directory is created.
* Default Permission for root and standard user:
  
| User           | Directory Permissions | File Permissions |
|----------------|-----------------------|------------------|
| Root           | 755                   | 644              |
| Standard User  | 775                   | 664              |

- Calculating Permission with Umask:

| User           | Calculation          | Umask | Umask Permission |
|----------------|----------------------|-------|------------------|
| Root Dir       | 777 - 022 = 755     | 022   | 755              |
| File           | 666 - 022 = 644     | 022   | 644              |
| Standard Dir   | 777 - 002 = 775     | 002   | 775              |
| File           | 666 - 002 = 664     | 002   | 664              |

