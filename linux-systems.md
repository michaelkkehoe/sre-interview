# Long-form Questions

* Describe the boot process of a Linux System
* Describe what happens when you type www.google.com into the Browser
* How does SSH Work
* Explain how eBPF works
* Explain how network packets are processed from the NIC to user-space
* Describe how a reimaging system works

# Short-form Questions
## Kernel
* What tasks are performed by the kernel
* What is Kernel-mode vs User-mode
* What is LD_LIBRARY_PATH
* What are the difference modes of network bonding
* Describe the /proc filesystem
* What are sysctl's

## File-System
* What are the various filesystem mount options and what do they do
* What are the basic file I/O methods
* What is a file descriptor
* What are the different types of IPC:
* What is an inode?
* How can you speed up accessing files?
* Where are filenames stored
* What is a Hard Link:
* What is a Soft Link:
* What is the /proc filesystem?
* What is the maximum length of a filename under linux?
* What are filenames that are preceded by a dot?
* What is a FIFO pipe?
* What is the difference between ext4 and ext3?

## Memory
* What is basic memory layout of a process

## Processes
*  Describe how processes are created
* What's the difference between fork/ clone?

## Resource Control
* What are the basic techniques for resource control?
## Capabilities
* CAP_AUDIT_CONTROL
*  CAP_AUDIT_READ
* CAP_AUDIT_WRITE
* CAP_BLOCK_SUSPEND
* CAP_CHOWN
* CAP_DAC_OVERRIDE
* CAP_DAC_READ_SEARCH
* CAP_FOWNER
* CAP_FSETID
* CAP_IPC_LOCK
* CAP_IPC_OWNER
* CAP_KILL
* CAP_LEASE (since Linux 2.4)
* CAP_LINUX_IMMUTABLE
* CAP_MAC_ADMIN (since Linux 2.6.25)
* CAP_MAC_OVERRIDE (since Linux 2.6.25)
* CAP_MKNOD (since Linux 2.4)
* CAP_NET_ADMIN
* CAP_NET_BIND_SERVICE
* CAP_NET_RAW
* CAP_SETGID
* CAP_SETFCAP (since Linux 2.6.24)
* CAP_SETPCAP
* CAP_SETUID
* CAP_SYS_ADMIN
* CAP_SYS_BOOT
* CAP_SYS_CHROOT
* CAP_SYS_MODULE
* CAP_SYS_NICE
* CAP_SYS_PACCT
* CAP_SYS_PTRACE
* CAP_SYS_RAWIO
* CAP_SYS_RESOURCE
* CAP_SYS_TIME
* CAP_SYS_TTY_CONFIG
* CAP_SYSLOG
* CAP_WAKE_ALARM
              
## Linux history
* What is POSIX
* What is the GNU Project
* What is the standard C library

## Syscalls
* accept (2)           - accept a connection on a socket
* accept4 (2)          - accept a connection on a socket
* access (2)           - check real user's permissions for a file
* acct (2)             - switch process accounting on or off
* add_key (2)          - add a key to the kernel's key management facility
* adjtimex (2)         - tune kernel clock
* alarm (2)            - set an alarm clock for delivery of a signal
* alloc_hugepages (2)  - allocate or free huge pages
* arch_prctl (2)       - set architecture-specific thread state
* arm_fadvise (2)      - predeclare an access pattern for file data
* arm_fadvise64_64 (2) - predeclare an access pattern for file data
* arm_sync_file_range (2) - sync a file segment with disk
* bdflush (2)          - start, flush, or tune buffer-dirty-flush daemon
* bind (2)             - bind a name to a socket
* brk (2)              - change data segment size
* cacheflush (2)       - flush contents of instruction and/or data cache
* capget (2)           - set/get capabilities of thread(s)
* capset (2)           - set/get capabilities of thread(s)
* chdir (2)            - change working directory
* chmod (2)            - change permissions of a file
* chown (2)            - change ownership of a file
* chown32 (2)          - change ownership of a file
* chroot (2)           - change root directory
* clock_getres (2)     - clock and time functions
* clock_gettime (2)    - clock and time functions
* clock_nanosleep (2)  - high-resolution sleep with specifiable clock
* clock_settime (2)    - clock and time functions
* clone2 (2)           - create a child process
* clone2 (2)           - create a child process
* clone (2)            - create a child process
* close (2)            - close a file descriptor
* connect (2)          - initiate a connection on a socket
* creat (2)            - open and possibly create a file or device
* create_module (2)    - create a loadable module entry
* delete_module (2)    - unload a kernel module
* dup2 (2)             - duplicate a file descriptor
* dup (2)              - duplicate a file descriptor
* dup3 (2)             - duplicate a file descriptor
* epoll_create1 (2)    - open an epoll file descriptor
* epoll_create (2)     - open an epoll file descriptor
* epoll_ctl (2)        - control interface for an epoll descriptor
* epoll_pwait (2)      - wait for an I/O event on an epoll file descriptor
* epoll_wait (2)       - wait for an I/O event on an epoll file descriptor
* eventfd2 (2)         - create a file descriptor for event notification
* eventfd (2)          - create a file descriptor for event notification
* execve (2)           - execute program
* _exit (2)            - terminate the calling process
* exit (2)             - terminate the calling process
* _Exit (2)            - terminate the calling process
* exit_group (2)       - exit all threads in a process
* faccessat (2)        - check user's permissions of a file relative to a direc...
* fadvise64 (2)        - predeclare an access pattern for file data
* fadvise64_64 (2)     - predeclare an access pattern for file data
* fallocate (2)        - manipulate file space
* fanotify_init (2)    - create and initialize fanotify group
* fchdir (2)           - change working directory
* fchmod (2)           - change permissions of a file
* fchmodat (2)         - change permissions of a file relative to a directory f...
* fchown (2)           - change ownership of a file
* fchown32 (2)         - change ownership of a file
* fchownat (2)         - change ownership of a file relative to a directory fil...
* fcntl (2)            - manipulate file descriptor
* fcntl64 (2)          - manipulate file descriptor
* fdatasync (2)        - synchronize a file's in-core state with storage device
* finit_module (2)     - load a kernel module
* flock (2)            - apply or remove an advisory lock on an open file
* fork (2)             - create a child process
* free_hugepages (2)   - allocate or free huge pages
* fstat (2)            - get file status
* fstat64 (2)          - get file status
* fstatat (2)          - get file status relative to a directory file descriptor
* fstatat64 (2)        - get file status relative to a directory file descriptor
* fstatfs (2)          - get file system statistics
* fstatfs64 (2)        - get file system statistics
* fstatvfs (2)         - get file system statistics
* fsync (2)            - synchronize a file's in-core state with storage device
* ftruncate (2)        - truncate a file to a specified length
* ftruncate64 (2)      - truncate a file to a specified length
* futex (2)            - fast user-space locking
* futimesat (2)        - change timestamps of a file relative to a directory fi...
* getcontext (2)       - get or set the user context
* getcpu (2)           - determine CPU and NUMA node on which the calling threa...
* getcwd (2)           - get current working directory
* getdents (2)         - get directory entries
* getdents64 (2)       - get directory entries
* getdomainname (2)    - get/set NIS domain name
* getdtablesize (2)    - get descriptor table size
* getegid (2)          - get group identity
* getegid32 (2)        - get group identity
* geteuid (2)          - get user identity
* geteuid32 (2)        - get user identity
* getgid (2)           - get group identity
* getgid32 (2)         - get group identity
* getgroups (2)        - get/set list of supplementary group IDs
* getgroups32 (2)      - get/set list of supplementary group IDs
* gethostid (2)        - get or set the unique identifier of the current host
* gethostname (2)      - get/set hostname
* getitimer (2)        - get or set value of an interval timer
* get_kernel_syms (2)  - retrieve exported kernel and module symbols
* get_mempolicy (2)    - retrieve NUMA memory policy for a process
* getpagesize (2)      - get memory page size
* getpeername (2)      - get name of connected peer socket
* getpgid (2)          - set/get process group
* getpgrp (2)          - set/get process group
* getpid (2)           - get process identification
* getppid (2)          - get process identification
* getpriority (2)      - get/set program scheduling priority
* getresgid (2)        - get real, effective and saved user/group IDs
* getresgid32 (2)      - get real, effective and saved user/group IDs
* getresuid (2)        - get real, effective and saved user/group IDs
* getresuid32 (2)      - get real, effective and saved user/group IDs
* getrlimit (2)        - get/set resource limits
* get_robust_list (2)  - get/set list of robust futexes
* getrusage (2)        - get resource usage
* getsid (2)           - get session ID
* getsockname (2)      - get socket name
* getsockopt (2)       - get and set options on sockets
* get_thread_area (2)  - get a thread-local storage (TLS) area
* gettid (2)           - get thread identification
* gettimeofday (2)     - get / set time
* getuid (2)           - get user identity
* getuid32 (2)         - get user identity
* getunwind (2)        - copy the unwind data to caller's buffer
* idle (2)             - make process 0 idle
* inb (2)              - port I/O
* inb_p (2)            - port I/O
* init_module (2)      - load a kernel module
* inl (2)              - port I/O
* inl_p (2)            - port I/O
* inotify_add_watch (2) - add a watch to an initialized inotify instance
* inotify_init1 (2)    - initialize an inotify instance
* inotify_init (2)     - initialize an inotify instance
* inotify_rm_watch (2) - remove an existing watch from an inotify instance
* insb (2)             - port I/O
* insl (2)             - port I/O
* insw (2)             - port I/O
* intro (2)            - introduction to system calls
* inw (2)              - port I/O
* inw_p (2)            - port I/O
* io_cancel (2)        - cancel an outstanding asynchronous I/O operation
* ioctl (2)            - control device
* ioctl_list (2)       - list of ioctl calls in Linux/i386 kernel
* io_destroy (2)       - destroy an asynchronous I/O context
* io_getevents (2)     - read asynchronous I/O events from the completion queue
* ioperm (2)           - set port input/output permissions
* iopl (2)             - change I/O privilege level
* ioprio_get (2)       - get/set I/O scheduling class and priority
* ioprio_set (2)       - get/set I/O scheduling class and priority
* io_setup (2)         - create an asynchronous I/O context
* io_submit (2)        - submit asynchronous I/O blocks for processing
* ipc (2)              - System V IPC system calls
* kcmp (2)             - compare two processes to determine if they share a ker...
* kexec_load (2)       - load a new kernel for later execution
* keyctl (2)           - manipulate the kernel's key management facility
* kill (2)             - send signal to a process
* killpg (2)           - send signal to a process group
* lchown (2)           - change ownership of a file
* lchown32 (2)         - change ownership of a file
* link (2)             - make a new name for a file
* linkat (2)           - create a file link relative to directory file descriptors
* listen (2)           - listen for connections on a socket
* _llseek (2)          - reposition read/write file offset
* llseek (2)           - reposition read/write file offset
* lookup_dcookie (2)   - return a directory entry's path
* lseek (2)            - reposition read/write file offset
* lstat (2)            - get file status
* lstat64 (2)          - get file status
* madvise (2)          - give advice about use of memory
* mbind (2)            - set memory policy for a memory range
* migrate_pages (2)    - move all pages in a process to another set of nodes
* mincore (2)          - determine whether pages are resident in memory
* mkdir (2)            - create a directory
* mkdirat (2)          - create a directory relative to a directory file descri...
* mknod (2)            - create a special or ordinary file
* mknodat (2)          - create a special or ordinary file relative to a direct...
* mlock (2)            - lock and unlock memory
* mlockall (2)         - lock and unlock memory
* mmap2 (2)            - map files or devices into memory
* mmap (2)             - map or unmap files or devices into memory
* modify_ldt (2)       - get or set ldt
* mount (2)            - mount file system
* move_pages (2)       - move individual pages of a process to another node
* mprotect (2)         - set protection on a region of memory
* mq_getsetattr (2)    - get/set message queue attributes
* mq_notify (2)        - register for notification when a message is available
* mq_open (2)          - open a message queue
* mq_timedreceive (2)  - receive a message from a message queue
* mq_timedsend (2)     - send a message to a message queue
* mq_unlink (2)        - remove a message queue
* mremap (2)           - remap a virtual memory address
* msgctl (2)           - System V message control operations
* msgget (2)           - get a System V message queue identifier
* msgop (2)            - System V message queue operations
* msgrcv (2)           - System V message queue operations
* msgsnd (2)           - System V message queue operations
* msync (2)            - synchronize a file with a memory map
* munlock (2)          - lock and unlock memory
* munlockall (2)       - lock and unlock memory
* munmap (2)           - map or unmap files or devices into memory
* nanosleep (2)        - high-resolution sleep
* _newselect (2)       - synchronous I/O multiplexing
* nfsservctl (2)       - syscall interface to kernel nfs daemon
* nice (2)             - change process priority
* oldfstat (2)         - get file status
* oldlstat (2)         - get file status
* oldolduname (2)      - get name and information about current kernel
* oldstat (2)          - get file status
* olduname (2)         - get name and information about current kernel
* open (2)             - open and possibly create a file or device
* openat (2)           - open a file relative to a directory file descriptor
* outb (2)             - port I/O
* outb_p (2)           - port I/O
* outl (2)             - port I/O
* outl_p (2)           - port I/O
* outsb (2)            - port I/O
* outsl (2)            - port I/O
* outsw (2)            - port I/O
* outw (2)             - port I/O
* outw_p (2)           - port I/O
* pause (2)            - wait for signal
* perf_event_open (2)  - set up performance monitoring
* perfmonctl (2)       - interface to IA-64 performance monitoring unit
* personality (2)      - set the process execution domain
* pipe2 (2)            - create pipe
* pipe (2)             - create pipe
* pivot_root (2)       - change the root file system
* poll (2)             - wait for some event on a file descriptor
* posix_fadvise (2)    - predeclare an access pattern for file data
* ppoll (2)            - wait for some event on a file descriptor
* prctl (2)            - operations on a process
* pread (2)            - read from or write to a file descriptor at a given offset
* pread64 (2)          - read from or write to a file descriptor at a given offset
* preadv (2)           - read or write data into multiple buffers
* process_vm_readv (2) - transfer data between process address spaces
* process_vm_writev (2) - transfer data between process address spaces
* pselect (2)          - synchronous I/O multiplexing
* pselect6 (2)         - synchronous I/O multiplexing
* ptrace (2)           - process trace
* pwrite (2)           - read from or write to a file descriptor at a given offset
* pwrite64 (2)         - read from or write to a file descriptor at a given offset
* pwritev (2)          - read or write data into multiple buffers
* query_module (2)     - query the kernel for various bits pertaining to modules
* quotactl (2)         - manipulate disk quotas
* read (2)             - read from a file descriptor
* readahead (2)        - perform file readahead into page cache
* readdir (2)          - read directory entry
* readlink (2)         - read value of a symbolic link
* readlinkat (2)       - read value of a symbolic link relative to a directory ...
* readv (2)            - read or write data into multiple buffers
* reboot (2)           - reboot or enable/disable Ctrl-Alt-Del
* recv (2)             - receive a message from a socket
* recvfrom (2)         - receive a message from a socket
* recvmmsg (2)         - receive multiple messages on a socket
* recvmsg (2)          - receive a message from a socket
* remap_file_pages (2) - create a nonlinear file mapping
* rename (2)           - change the name or location of a file
* renameat (2)         - rename a file relative to directory file descriptors
* request_key (2)      - request a key from the kernel's key management facility
* restart_syscall (2)  - restart a system call after interruption by a stop signal
* rmdir (2)            - delete a directory
* rtas (2)             - Allows userspace to call RTAS (Run Time Abstraction Se...
* rt_sigaction (2)     - examine and change a signal action
* rt_sigpending (2)    - examine pending signals
* rt_sigprocmask (2)   - examine and change blocked signals
* rt_sigqueueinfo (2)  - queue a signal and data
* rt_sigreturn (2)     - return from signal handler and cleanup stack frame
* rt_sigsuspend (2)    - wait for a signal
* rt_sigtimedwait (2)  - synchronously wait for queued signals
* rt_tgsigqueueinfo (2) - queue a signal and data
* s390_runtime_instr (2) - enable/disable s390 CPU run-time instrumentation
* sbrk (2)             - change data segment size
* sched_getaffinity (2) - set and get a process's CPU affinity mask
* sched_getparam (2)   - set and get scheduling parameters
* sched_get_priority_max (2) - get static priority range
* sched_get_priority_min (2) - get static priority range
* sched_getscheduler (2) - set and get scheduling policy/parameters
* sched_rr_get_interval (2) - get the SCHED_RR interval for the named process
* sched_setaffinity (2) - set and get a process's CPU affinity mask
* sched_setparam (2)   - set and get scheduling parameters
* sched_setscheduler (2) - set and get scheduling policy/parameters
* sched_yield (2)      - yield the processor
* select (2)           - synchronous I/O multiplexing
* select_tut (2)       - synchronous I/O multiplexing
* semctl (2)           - System V semaphore control operations
* semget (2)           - get a System V semaphore set identifier
* semop (2)            - System V semaphore operations
* semtimedop (2)       - System V semaphore operations
* send (2)             - send a message on a socket
* sendfile (2)         - transfer data between file descriptors
* sendfile64 (2)       - transfer data between file descriptors
* sendmmsg (2)         - send multiple messages on a socket
* sendmsg (2)          - send a message on a socket
* sendto (2)           - send a message on a socket
* setcontext (2)       - get or set the user context
* setegid (2)          - set effective user or group ID
* seteuid (2)          - set effective user or group ID
* setfsgid (2)         - set group identity used for file system checks
* setfsgid32 (2)       - set group identity used for file system checks
* setfsuid (2)         - set user identity used for file system checks
* setfsuid32 (2)       - set user identity used for file system checks
* setgid (2)           - set group identity
* setgid32 (2)         - set group identity
* setgroups (2)        - get/set list of supplementary group IDs
* setgroups32 (2)      - get/set list of supplementary group IDs
* sethostid (2)        - get or set the unique identifier of the current host
* sethostname (2)      - get/set hostname
* setitimer (2)        - get or set value of an interval timer
* set_mempolicy (2)    - set default NUMA memory policy for a process and its c...
* setns (2)            - reassociate thread with a namespace
* setpgid (2)          - set/get process group
* setpgrp (2)          - set/get process group
* setpriority (2)      - get/set program scheduling priority
* setregid (2)         - set real and/or effective user or group ID
* setregid32 (2)       - set real and/or effective user or group ID
* setresgid (2)        - set real, effective and saved user or group ID
* setresgid32 (2)      - set real, effective and saved user or group ID
* setresuid (2)        - set real, effective and saved user or group ID
* setresuid32 (2)      - set real, effective and saved user or group ID
* setreuid (2)         - set real and/or effective user or group ID
* setreuid32 (2)       - set real and/or effective user or group ID
* set_robust_list (2)  - get/set list of robust futexes
* setsid (2)           - creates a session and sets the process group ID
* setsockopt (2)       - get and set options on sockets
* set_thread_area (2)  - set a thread local storage (TLS) area
* set_tid_address (2)  - set pointer to thread ID
* settimeofday (2)     - get / set time
* setuid (2)           - set user identity
* setuid32 (2)         - set user identity
* setup (2)            - setup devices and file systems, mount root file system
* sgetmask (2)         - manipulation of signal mask (obsolete)
* shmat (2)            - System V shared memory operations
* shmctl (2)           - System V shared memory control
* shmdt (2)            - System V shared memory operations
* shmget (2)           - allocates a System V shared memory segment
* shmop (2)            - System V shared memory operations
* shutdown (2)         - shut down part of a full-duplex connection
* sigaction (2)        - examine and change a signal action
* sigaltstack (2)      - set and/or get signal stack context
* signal (2)           - ANSI C signal handling
* signalfd (2)         - create a file descriptor for accepting signals
* signalfd4 (2)        - create a file descriptor for accepting signals
* sigpending (2)       - examine pending signals
* sigprocmask (2)      - examine and change blocked signals
* sigqueue (2)         - queue a signal and data to a process
* sigreturn (2)        - return from signal handler and cleanup stack frame
* sigsuspend (2)       - wait for a signal
* sigtimedwait (2)     - synchronously wait for queued signals
* sigwaitinfo (2)      - synchronously wait for queued signals
* socket (2)           - create an endpoint for communication
* socketcall (2)       - socket system calls
* socketpair (2)       - create a pair of connected sockets
* splice (2)           - splice data to/from a pipe
* spu_create (2)       - create a new spu context
* spu_run (2)          - execute an SPU context
* ssetmask (2)         - manipulation of signal mask (obsolete)
* stat (2)             - get file status
* stat64 (2)           - get file status
* statfs (2)           - get file system statistics
* statfs64 (2)         - get file system statistics
* statvfs (2)          - get file system statistics
* stime (2)            - set time
* subpage_prot (2)     - define a subpage protection for an address range
* swapcontext (2)      - Swap out old context with new context
* swapoff (2)          - start/stop swapping to file/device
* swapon (2)           - start/stop swapping to file/device
* symlink (2)          - make a new name for a file
* symlinkat (2)        - create a symbolic link relative to a directory file de...
* sync (2)             - commit buffer cache to disk
* sync_file_range2 (2) - sync a file segment with disk
* sync_file_range (2)  - sync a file segment with disk
* syncfs (2)           - commit buffer cache to disk
* syscall (2)          - indirect system call
* _syscall (2)         - invoking a system call without library support (OBSOLETE)
* syscalls (2)         - Linux system calls
* _sysctl (2)          - read/write system parameters
* sysctl (2)           - read/write system parameters
* sysfs (2)            - get file system type information
* sysinfo (2)          - returns information on overall system statistics
* syslog (2)           - read and/or clear kernel message ring buffer; set cons...
* tee (2)              - duplicating pipe content
* tgkill (2)           - send a signal to a thread
* time (2)             - get time in seconds
* timer_create (2)     - create a POSIX per-process timer
* timer_delete (2)     - delete a POSIX per-process timer
* timerfd_create (2)   - timers that notify via file descriptors
* timerfd_gettime (2)  - timers that notify via file descriptors
* timerfd_settime (2)  - timers that notify via file descriptors
* timer_getoverrun (2) - get overrun count for a POSIX per-process timer
* timer_gettime (2)    - arm/disarm and fetch state of POSIX per-process timer
* timer_settime (2)    - arm/disarm and fetch state of POSIX per-process timer
* times (2)            - get process times
* tkill (2)            - send a signal to a thread
* truncate (2)         - truncate a file to a specified length
* truncate64 (2)       - truncate a file to a specified length
* ugetrlimit (2)       - get/set resource limits
* umask (2)            - set file mode creation mask
* umount2 (2)          - unmount file system
* umount (2)           - unmount file system
* uname (2)            - get name and information about current kernel
* unlink (2)           - delete a name and possibly the file it refers to
* unlinkat (2)         - remove a directory entry relative to a directory file ...
* unshare (2)          - disassociate parts of the process execution context
* uselib (2)           - load shared library
* ustat (2)            - get file system statistics
* utime (2)            - change file last access and modification times
* utimensat (2)        - change file timestamps with nanosecond precision
* utimes (2)           - change file last access and modification times
* vfork (2)            - create a child process and block parent
* vhangup (2)          - virtually hangup the current terminal
* vm86 (2)             - enter virtual 8086 mode
* vm86old (2)          - enter virtual 8086 mode
* vmsplice (2)         - splice user pages into a pipe
* wait (2)             - wait for process to change state
* wait3 (2)            - wait for process to change state, BSD style
* wait4 (2)            - wait for process to change state, BSD style
* waitid (2)           - wait for process to change state
* waitpid (2)          - wait for process to change state
* write (2)            - write to a file descriptor
* writev (2)           - read or write data into multiple buffers

## Commands
* What are the different shells
