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
## Resource Control
* What are the basic techniques for resource control?
  * CGroups
  * limits.conf
  * CPU affinity
## Capabilities
## Linux history
* What is POSIX
* What is the GNU Project
* What is the standard C library
## Syscalls
## Commands
* What are the different shells
  * Bourne Shell (sh)
  * C Shell (csh)
  * Korn Shell (ksh)
  * Bourne again Shell (BASH)

