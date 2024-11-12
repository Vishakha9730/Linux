# Namespaces -
- Linux namespaces are a way to create isolated environments within a single Linux system.
- These isolated environments allow processes to think they are running on their own independent machine, even though they are sharing the same physical system.
- Namespaces are a feature of the Linux kernel that partition kernel resources such that one set of processes sees one set of resources, while another set of processes sees a different set of resources.

 # Types of Namespaces -
 ### 1] PID namespace: 
 - Isolates process IDs.
 - Each set of processes in a PID namespace has its own numbering for processes, so a process in one namespace can have a PID of 1, while another process in another namespace might also have PID 1.

### 2] Network namespace: 
- Isolates network resources like IP addresses, network interfaces, routing tables, etc.
- Processes in different network namespaces don't see each other's network settings, which is useful for containers that need separate network configurations.

### 3] Mount namespace: 
- Isolates file system mounts.
- Processes in different mount namespaces can have different views of the filesystem.
- For example, one namespace might have /home mounted on one location, while another namespace might have it mounted somewhere else.





