1. What is Linux.
 
Linux is a kernel. 
It is free to use, open-source, and highly customizable.
linux is a open source thats why we can use it and create a new operating system.
linux is created by LINUS TORVALD in 17 september 1991.
Linux let the hordware and software work together with smoothly on our device.

2. What is kernel.
     
The kernel is the core part of an operating system. It acts as a bridge between the hardware and software, managing system resources like CPU, memory, and devices. It also helps applications communicate with the hardware without needing to know the details of how the hardware works.

3. Types of Kernel.
 
There are mainly two types of kernels:
**1. Monolithic Kernel:** In this type, the entire operating system runs in the kernel space. In monolithic kernel user and monolithic serices are kept in same address space.
**2. Microkernel:** In a microkernel system, only the essential functions, like communication between hardware and software, run in the kernel space. Other services, like device drivers and file management, run in user space. In microkernel user services and kernel services are kept in separate address space.

4. which kernel we use in linux ?
 
We use Monolithic kernel in linux.

5. what is virtualization ?
 
Vertualization is technology that lets us to create multiple virtual machine on a single physical server. virtualization allows you to run many operating systems or applications at the same time. Each virtual environment behaves like its own separate machine, even though they are all sharing the same hardware.

7. what is Hyperviosor ?

A hypervisor is software that allows you to create and run virtual machines (VMs) on a physical computer. It acts as a middle layer between the physical hardware and the virtual machines. Each VM runs its own operating system, and the hypervisor makes sure that all VMs can share the physical resources like CPU, memory, and storage without interfering with each other.
  there are two type of Hypervisor. first one is Type 1 Bare metal This type runs directly on the physical hardware.It's often used in large data centers. then second one is Type2 Hosted This type runs on top of an existing operating system like Windows or Linux. It's more commonly used on personal computers.

9. what is shell ?

A shell is a program that provides an interface for users to interact with the operating system. It allows you to run commands, execute scripts, and manage files or processes. You can think of it as a bridge between the user and the computer's operating system.

11. Difference between Windows and linux.

12. what is operating system ?

An operating system (OS) is the main software that runs on a computer and manages both the hardware and software. It acts as a bridge between the user and the computer hardware, helping to run applications, manage files, and control devices like the CPU, memory, and storage.

14. Architecture of linux.


15. What is Relative path and Absolute path ?

A relative path is a path that starts from the current working directory. It does not include the full path from the root but instead uses a shortcut based on where you currently are. An absolute path is a full path that starts from the root directory of the filesystem. It provides the complete address to a file or directory.

16. Which Hypervisor we use in linux and AWS ?

I used VMware and VirtualBox in Linux and AWS uses the Xen hypervisor for most of its instances, but it has also started using Nitro for newer instance types, which provides better performance and security.

17. Explain Hirarchy ?


18. Explain classification of OS ?

single user single tasking, single user multy tasking, multy user single tasking, multy user multy tasking. 

19. what is the difference between /root & /home ?

/root: Home directory of the root user (superuser), located directly under `/`, with access restricted to the root user. /home: Directory containing home directories of all regular users, with each user having their own folder (e.g., `/home/username`). Regular users have access only to their own directories.

20. Explain Boot process ?

21. explain vim editor. 

vim is a very powerful and configurable editor in Linux system. it's very simple when we learned shortcut in that. 

22. Modes of Vim editor. 

there are four modes in vim editor: first one is Normal mode for navigate and edit text then second is insert mode for write a text later third is visual mode for selecting the text and last one is command mode for perform action like saving, quiting or searching. 

23. how to check the kernel and kernel version ?

We can see the kernel and krnel verison with the command like `uname`, `uname -r`, `uname -sr`

24. how to check the machine we use?

we can check the machine we use with `cat /etc/os-release`, `lsb_release -a`

25. how to check memory ?

we check the memory using `free` command in that we can see memory and swap memory also.

26. how to check the storage ?

we check the storage using `df -hT` command.

27. how to check shell we use ?

we can check the shell we use with `echo $SHELL` & `echo $0`

28. where is stored the shells ?

shell stored at /etc/shells.

29. Explain Redirectors ?

we use redirector to append output or error in files with its type like >, >>, 2>, 2>>, &> and &>>. in that when we use single redirector that time it overwrite with previous text or error and when we use >> redirector that time my old text and new text or error both are saved in that file.

30. 7 entries of user when its create ?

when we add user in linux system its been create a 7 entries.
- /home/username
- /etc/passwd
- /etc/group
- /etc/shadow
- /etc/gshadow
- /wtc/skel
- /var/spool/mail

31. Field of passwd ?

uname:link of encrypted password:uid:gid:comment:home directory of user:shell 

32. field of group & gshadow.

Field of Group : group name:Link of encrypted passwd:Gid:Members in group
Field of gshadow : group name:Link of encrypted passwd:Gid:Members in group 

33. field of shadow ?

username:encryptedpasswd:lastchangepasswd:Minimum password age:maximum password age:password expiry worning:Password Inactivity Period:Account Expiry Date:Reserved for future use

34. what is skelton file ?

the skeleton file is refers to a set of defaults file and configurations that are automatically copied at new users home directory when user created. These skeleton files are typically located in the /etc/skel directory. When a new user is added to the system using tools like useradd, the contents of /etc/skel are copied to the new user's home directory. This ensures that each user starts with the same initial setup, such as default configuration files for shells, editors, or other programs. Common Skeleton Files: `.bashrc` A configuration file for the bash shell. `.profile` A user profile script for environment settings.`.bash_logout` Script run when logging out of a bash shell.

35. what is the difference between useradd and adduser ?

useradd is a low level command It does not set up default directories, user passwords, or other user-specific configurations. and adduser is a higher level command It provides an interactive process, asking for the user's password, full name, home directory, default shell.  adduser automatically creates a home directory, whereas useradd needs the -m flag to do so.

36. UID of system user, root user, local user.

Root user uid : 0     #
System User uid : 1 - 999
Local user uid : 1000 +   $

37. what is metadata ?

Metadata is data that provides information about other data. In a file system, metadata includes details like file name, size, creation date, and permissions, but not the file's content.

38. what is the purpose of user management ?

The purpose of user management is to control who can access a system and what they can do. It ensures that each person has the right permissions based on their job or role. By managing users properly, you keep the system secure, make sure resources are used correctly, and can track what each user is doing.

39. what is the purpose of group management ?

The purpose of group management is to make it easier to manage user permissions by organizing users into groups. Instead of giving permissions to each person one by one, administrators can give permissions to a group, and everyone in that group gets the same access. This saves time and makes it simpler to control who can access certain resources.

40. where is the store password and link of password ?

stored password in /etc/passwd and /etc/group  and stored link of password in /etc/shadow/ and /etc/gshadow.

41. how to hide and unhide link of password ?

we can hide and unhide link of password usin `pwconv` and `pwunconv`. 

42. what is the link count of file and directory ?

In linux file system link count of file is `1` and link count of directory is `2`.

43. Explain permission management ?

In Linux permissions we can modify the permission of files and directories means define who access the file or directory. in that we can give three ways of permissions first one is READ for allow the read file content, second is Write for the Allows modifying or deleting the file and last is Execute Allows running the file as a program or script.
then we assign permission to owner, group and others then we difine ownership. in permission management we can define permission with numeric and also symbolic. we can change ownership with `chown` command and give the permission with `chmod` command. we also give a granular permission to user of specific file using ACL. 

44. Field of file.

- type of file
- owner permission
- group permission
- other permission
- Link count
- owner
- group
- Size
- timstamp
- name of file 

45. what is inode number and how to check it ?

An inode number is a unique identifier assigned to each file or directory in a filesystem on Unix-like operating systems, including Linux. It contains metadata about the file or directory but not the filename or the actual data content. and we can check inode number with command `ls -i`.

46. type of files.

there are seven types of files it classified into two type first one is User Define files and System define files. User define files is normal file(-), directory file(d), link file(l) and then system define files is block device file(b), pipe or fifo file(p), charachter file(c) and socket file(s). A user define files is executable from user and system define file is default by system.

47. what is chmod , chown , chgrp , chage ?

chmod: Changes file or directory permissions.
chown: Changes file or directory ownership.
chgrp: Changes the group ownership of a file or directory.
chage: Manages password expiry information for users.

48. how many ways to give permission ?

Permissions in Linux can be set in three ways: read, write, and execute. These permissions are assigned to three categories: owner, group, and others.

49. difference between Hardlink & Softlink.



50. what is newgrp command ?

The newgrp command allows you to switch to a different group within your current session, so you can access or modify files with the permissions of that group.

51. what is the purpose of ACL ?

The purpose of Access Control list in Linux to assign at Granular level permission to user, group on file and directory. we can assign permission of file to a single user or group.

52. why we use umask and desrcribe umask of root & local user ?

We use umask in linux system to set default permissin to newly created file and directory. but it deoends on user which user set or create a file or directory. 
the default umask of root user is 022 and umask of local user is 002. when root user create a directory its default permission is 755 and when create file its default permission is 644. and when local user create a directory its default permission is 775 and when its create a file then its default permission is 664. we can set umask set default permission for newly created file or directories. we also set umask permanent.

53. Explain Special permissions ?

"We use special permissions to offer more control over files and directories. There are three types of special permissions. SUID (Set User ID), SGID (Set Group ID) and  Sticky Bit. When we set SUID on a file, all users executing that file will have the file owner's privileges, often root. This allows normal users to perform tasks that require elevated privileges then after When SGID is assigned to a directory, any file or directory created inside will inherit the parent directory's group, not the user's default group. This is useful for maintaining group ownership consistency in shared directories later When the Sticky Bit is set on a directory, users cannot delete or modify files that they do not own, even if they have write permissions to the directory. Only the file owner or the root user can delete or modify their own files. 

54. what is sudoers file ?

The sudoers file is a configuration file in Linux that controls which users or groups have permission to run commands as the superuser (root) or another user, using sudo. It’s located at /etc/sudoers.

55. Port numbers ?

    - NFS -> 2049
    - FTP -> 20 & 21
    - SMTP -> 25
    - JENKINS -> 8080
    - MARIADB -> 3306
    - POSTGRESQL -> 5432
    - IMAP -> 143
    - NODEJS -> 3000
    - GRAFANA -> 3000
    - REACTS -> 3000
    - TOMCAT -> 8080
    - PROMETHEUS -> 9090
    - NODE EXPORTER -> 9091
    - SONARQUBE -> 9000

57. explain job scheduling ?

In linux job scheduling let us to automate the task at specific time which we set. In job scheduling Two tool for configure jobs first one is cron and second is at. cron is periodic schedular means its can execute multiple times we scheduled cron job with five fuilds `minute`, `Hour`, `Day of month`, `Month`, `week of the day`. and at is a nonperiodic means it execute at single time. 

58. difference between cron and at ?


59. Field of crontab ?

- minute of hour
- hour of day
- day of month
- month of year
- week of the day

60. Explain Search Filter & Utility commands ?



61. what is Archiving and Compression ?

Archiving is the process of collecting multiple files into a single file (an archive) to make storage or transfer easier. And Compression use to reduce file size of files or an archive to save space or make it quicker to transfer over networks.Often, archiving and compression are used together: you archive files into one file and then compress that file to save space. we compress files using gzip, bzip2 and xz. in xz possibilities to data losses.  

62. explain type of compression ?

there are three type of compression gzip, bzip2 and xzip. all compression is use to compress the archive file but in xzip posibilities of data losses. we use gunzip, bunzip2 and unxz to decompress the file.

63. what is Firewall ?

A firewall is a network security device or software that monitors and controls incoming and outgoing network traffic based on predetermined security rules. Its primary purpose is to create a barrier between a trusted internal network and untrusted external networks, such as the internet. firewalls are essential for maintaining network security by regulating traffic and protecting systems from attacks."

64. what is package management ?

Package management is the process of handling software packages in a Linux system. It involves installing, upgrading, configuring, and removing software applications and their dependencies. in that we use package manager like apt and yum, apt is used in Debian based distribution like ubuntu and yum is used in Red Hat based distribution like CentOS.

65. diffrence between yum & rpm.
66. diffrence btween `curl` & `wget`.



67. what is process management ?

Process management is refers to manage the process of operating system. manage the processes like creating , scheduling and terminating. in that we also set the nice value for configure priority of processes and range of nice value is -20 to 19. 

67. what is process id ?

In process management, a Process ID (PID) is a unique numerical identifier assigned by the operating system to each running process. The PID is used by the system to keep track of processes and manage them efficiently.

68. what is nice value and priority ?

the nice value is a setting that allows users to adjust the priority of a process. It affects how much CPU time that process gets compared to others. The nice value can range from -20 (highest priority) to 19 (lowest priority), with 0 as the default. A lower nice value means the process will run faster and get more CPU time, while a higher nice value means it will run slower and get less CPU time. By changing the nice value, users can help manage system performance. 

69. how to kill process id ?

We can kill the process with `kill` command using process id. like `kill -9 <PID>`

70. what is foreground and background (demonset) process.
71. what is Zombie ?
72. what is Load Average ?
73. Fields of `top` command.

A foreground process is one that interacts directly with the user. It occupies the terminal, and you can give it inputs, while it outputs data directly to the screen.You must wait for the process to complete before entering new commands in the terminal. A background process runs without user interaction and allows you to continue using the terminal for other tasks. These processes are usually started with an `&` symbol. You can run multiple tasks without waiting for one to finish.

71. what is Networking and its type ?

Networking refers to the practice of connecting computers and other devices together to share resources, exchange data, and communicate. It involves the design, implementation, and management of connections between devices in a network. there are some types of Network like personal area network for communicate betwwen personal devices like our phone connect with blutooth then Local Area Network for connects devices within a limited geographic area, such as a home, school, or office building. then after Metropoliton Area Network to connects devices across a city or a large campus, It's often used by organizations or municipalities to connect multiple buildings. then Wide Area Network for connect a large geographic area, connecting multiple LANs. It can connect cities, countries even all over worlds.

72. explain some componants of Network ?

I have knowledge about some componants like Routers for Connect different networks and route data packets between them, then Switch to Connect multiple devices within the same network (LAN) and forward data to specific devices based on their MAC addresses. then after Network Interface Card for Hardware that enables a device to connect to a network. NICs can be wired (Ethernet) or wireless (Wi-Fi). then after Bridge to Connect two or more network segments, allowing them to function as a single network. A bridge connecting two separate LANs in a building. These components work together to create and maintain a network, enabling communication and data exchange between devices

73. Explain OSI model.



74. difference between public and private ip.
75. rages of private ip.
76. ranges of public ip.
77. explain IP adrressing.
78. Difference between IPV4 & IPV6.
79. Reserved IP in Linux.
80. what is range of port.
81. what is broadcast ip ?
82. Explain TCP and its work ?
83. difference between TCP & UDP.
84. How to check private ip ?
85. how to check public ip ?
86. what is CIDR ?
87. where is store at files which we created.
88. where is store cron files which we created.
