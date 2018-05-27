# Long-form Questions

* Describe the boot process of a Linux System
  * See [https://github.com/nu11secur1ty/All-Stages-of-Linux-Booting-Process-](https://github.com/nu11secur1ty/All-Stages-of-Linux-Booting-Process-)
* Describe what happens when you type www.google.com into the Browser
  * See [https://github.com/alex/what-happens-when](https://github.com/alex/what-happens-when)
* How does SSH Work
  * See [https://www.slashroot.in/secure-shell-how-does-ssh-work](https://www.slashroot.in/secure-shell-how-does-ssh-work)
  
# Short-form Questions
## Kernel
* What tasks are performed by the kernel
  * Process scheduling
  * Memory management
  * Provision of filesystem
  * Creation and termination of proccesses
  * Access to devices
  * Networking
  * Provision of system call application programming
* What is Kernel-mode vs User-mode
  * When in user mode, CPU can only access memory marked for user space
  * When in Kernel mode, CPU can access memory in kernel & user space
## File-System
* What are the basic file I/O methods
  * open
  * read
  * write
  * close
* What is a file descriptor
* What are the different types of IPC:
  * Signals
  * Pipes
  * Sockets
  * File locking
  * Message Queues
  * Semaphores
  * Shared memory
* What is a Hard Link:
  * Hard link is the exact replica of the actual file it is pointing to. Both the hard link and the linked file shares the same inode.
* What is a Soft Link:
  * Symbolic link (Symlinks/Soft links) are links between files. It is nothing but a shortcut of a file (in windows terms).
* What is the /proc filesystem?
  * The proc filesystem (procfs) is a special filesystem in Unix operating systems that presents information about processes and other information in a hierarchial file-like structure, providing a more convienient and standardized method for dynamically accessing process data held in the kernel. 
* What is the maximum length of a filename under linux?
  * This is based on the filesystem. Generally it’s 255 bytes for the filename
* What are filenames that are preceded by a dot?
  * In general, filenames that are preceded by a dot are hidden files. These files can be configuration files that hold important data or setup info. Setting these files as hidden makes it less likely to be accidentally deleted.  
## Memory
* Process memory layout
  * Text: the instructions of the program
  * Data: The static variables
  * Heap: The area from which programs can dynamically allocate extra memory
  * Stack: A piece of memory that grows and shrinks as functions are called and return and that is used to allocate storage for local variables and function call linkage information
## Processes
*  Describe how processes are created
* What's the difference between fork/ clone?
## Resource Control
* What are the basic techniques for resource control?
  * CGroups
  * limits.conf
  * CPU affinity
## Capabilities
## Linux history
* What is POSIX
  * Portable Operating Systen Interface is a family standards specified by IEEE for maintaining compatability between UNIX systems. POSIX.1-2008 is one example of a standard.
* What is the GNU Project
* What is the standard C library
## Syscalls
* accept, accept4 - accept a connection on a socket
* access, faccessat - check user's permissions for a file
* acct - switch process accounting on or off
* add_key - add a key to the kernel's key management facility
* adjtimex, ntp_adjtime - tune kernel clock
* alarm - set an alarm clock for delivery of a signal
* bind - bind a name to a socket
* bpf - perform a command on an extended BPF map or program
* brk, sbrk - change data segment size
* cacheflush - flush contents of instruction and/or data cache
* capget, capset - set/get capabilities of thread(s)
* chdir, fchdir - change working directory
* chmod, fchmod, fchmodat - change permissions of a file
* chown, fchown, lchown, fchownat - change ownership of a file
* chroot - change root directory
* clock_getres - finds the resolution (precision) of the specified clock
* clock_gettime, clock_settime - retrieve and set the time of the specified clock clk_id
* clock_nanosleep - high-resolution sleep with specifiable clock
* clone, clone2 - create a child process
* close - close a file descriptor
* connect - initiate a connection on a socket
* copy_file_range - Copy a range of data from one file to another
* open, openat, creat - open and possibly create a file
* delete_module - unload a kernel module
* dup, dup2, dup3 - duplicate a file descriptor
* epoll_create, epoll_create1 - open an epoll file descriptor
* epoll_ctl - control interface for an epoll file descriptor
* epoll_wait,  epoll_pwait  -  wait  for  an I/O event on an epoll file descriptor
* eventfd - create a file descriptor for event notification
* execve - execute program
* execveat - execute program relative to a directory file descriptor
* _exit, _Exit - terminate the calling process
* exit_group - exit all threads in a process
* access, faccessat - check user's permissions for a file
* posix_fadvise - predeclare an access pattern for file data
* fallocate - manipulate file space
* fanotify_init - create and initialize fanotify group
* fanotify_mark - add, remove, or modify an fanotify mark on a filesystem object
* fcntl - manipulate file descriptor
* fsync,  fdatasync  -  synchronize a file's in-core state with storage device
* getxattr, lgetxattr, fgetxattr - retrieve an extended attribute value
* init_module, finit_module - load a kernel module
* listxattr, llistxattr, flistxattr - list extended attribute names
* flock - apply or remove an advisory lock on an open file
* fork - create a child process
* removexattr, lremovexattr, fremovexattr - remove an extended attribute
* setxattr, lsetxattr, fsetxattr - set an extended attribute value
* stat, fstat, lstat, fstatat - get file status
* statfs, fstatfs - get filesystem statistics
* fsync, fdatasync - synchronize a file's in-core state with storage device
* truncate, ftruncate - truncate a file to a specified length
* futex - fast user-space locking
* futimesat  - change timestamps of a file relative to a directory file descriptor
* get_mempolicy - retrieve NUMA memory policy for a thread
* get_robust_list, set_robust_list - get/set list of robust futexes
* get_thread_area,  set_thread_area  - set a GDT entry for thread-local storage
* getcpu - determine CPU and NUMA node on which the calling thread is running
* getcwd, getwd, get_current_dir_name - get current working directory
* getdents, getdents64 - get directory entries
* getgid, getegid - get group identity
* getuid, geteuid - get user identity
* getgid, getegid - get group identity
* getgroups, setgroups - get/set list of supplementary group IDs
* getitimer, setitimer - get or set value of an interval timer
* getpeername - get name of connected peer socket
* setpgid, getpgid, setpgrp, getpgrp - set/get process group
* setpgid, getpgid, setpgrp, getpgrp - set/get process group
* getpid, getppid - get process identification
* getpid, getppid - get process identification
* getpriority, setpriority - get/set program scheduling priority
* getrandom - obtain a series of random bytes
* getresuid, getresgid - get real, effective and saved user/group IDs
* getresuid, getresgid - get real, effective and saved user/group IDs
* getrlimit, setrlimit, prlimit - get/set resource limits
* getrusage - get resource usage
* getsid - get session ID
* getsockname - get socket name
* getsockopt, setsockopt - get and set options on sockets
* gettid - get thread identification
## Commands
* What are the different shells
  * Bourne Shell (sh)
  * C Shell (csh)
  * Korn Shell (ksh)
  * Bourne again Shell (BASH)
