## Linux Security

*Q: What are some Linux Security Modules?*

A: List below

* App Armor
* SELinux
* Smack
* TOMOYO
* eBPF

*Q: What are the Linux Capabilities?*

A: List Below:

* CAP_AUDIT_CONTROL
  * Enable and disable kernel auditing
  * change auditing filter rules
  * retrieve auditing status and filtering rules.
*  CAP_AUDIT_READ
  * Allow reading the audit log via a multicast netlink socket.
* CAP_AUDIT_WRITE
  * Write records to kernel auditing log.
* CAP_BLOCK_SUSPEND
  * Employ features that can block system suspend (epoll(7) EPOLLWAKEUP, /proc/sys/wake_lock).
* CAP_CHOWN
  * Make arbitrary changes to file UIDs and GIDs (see chown(2)).
* CAP_DAC_OVERRIDE
  * Bypass file read, write, and execute permission checks.  (DAC is an abbreviation of "discretionary access control".)
* CAP_DAC_READ_SEARCH
  * Bypass file read permission checks and directory read and execute permission checks;
  * invoke open_by_handle_at(2);
  * use the linkat(2) AT_EMPTY_PATH flag to create a link to a file referred to by a file descriptor.
* CAP_FOWNER
  * Bypass permission checks on operations that normally require the filesystem UID of the process to match the UID of the file (e.g., chmod(2), utime(2)), excluding those operations covered by CAP_DAC_OVERRIDE and CAP_DAC_READ_SEARCH;
  * set inode flags (see ioctl_iflags(2)) on arbitrary files;
  * set Access Control Lists (ACLs) on arbitrary files;
  * ignore directory sticky bit on file deletion;
  * specify O_NOATIME for arbitrary files in open(2) and fcntl(2).
* CAP_FSETID
  * Don't clear set-user-ID and set-group-ID mode bits when a file is modified;
  * set the set-group-ID bit for a file whose GID does not match the filesystem or any of the supplementary GIDs of the calling process.
* CAP_IPC_LOCK
  * Lock memory (mlock(2), mlockall(2), mmap(2), shmctl(2)).
* CAP_IPC_OWNER
  * Bypass permission checks for operations on System V IPC objects.
* CAP_KILL
  * Bypass permission checks for sending signals (see kill(2)). This includes use of the ioctl(2) KDSIGACCEPT operation.
* CAP_LEASE (since Linux 2.4)
  * Establish leases on arbitrary files (see fcntl(2)).
* CAP_LINUX_IMMUTABLE
  * Set the FS_APPEND_FL and FS_IMMUTABLE_FL inode flags (see ioctl_iflags(2)).
* CAP_MAC_ADMIN (since Linux 2.6.25)
  * Allow MAC configuration or state changes.  Implemented for the Smack Linux Security Module (LSM).
* CAP_MAC_OVERRIDE (since Linux 2.6.25)
  * Override Mandatory Access Control (MAC).  Implemented for the  Smack LSM.
* CAP_MKNOD (since Linux 2.4)
   * Create special files using mknod(2).
* CAP_NET_ADMIN
  * Perform various network-related operations:
  * interface configuration;
  * administration of IP firewall, masquerading, and accounting;
  * modify routing tables;
  * bind to any address for transparent proxying;
  * set type-of-service (TOS)
  * clear driver statistics;
  * set promiscuous mode;
  * enabling multicasting;
  * use setsockopt(2) to set the following socket options: SO_DEBUG, SO_MARK, SO_PRIORITY (for a priority outside the range 0 to 6), SO_RCVBUFFORCE, and SO_SNDBUFFORCE.
* CAP_NET_BIND_SERVICE
  * Bind a socket to Internet domain privileged ports (port numbers less than 1024).
* CAP_NET_RAW
  * Use RAW and PACKET sockets;
  * bind to any address for transparent proxying.
* CAP_SETGID
  * Make arbitrary manipulations of process GIDs and supplementary GID list;
  * forge GID when passing socket credentials via UNIX domain sockets;
  * write a group ID mapping in a user namespace (see user_namespaces(7)).
* CAP_SETFCAP (since Linux 2.6.24)
  * Set arbitrary capabilities on a file.
* CAP_SETPCAP
  *  If file capabilities are supported (i.e., since Linux 2.6.24): add any capability from the calling thread's bounding set to its inheritable set; drop capabilities from the bounding set (via prctl(2) PR_CAPBSET_DROP); make changes to the securebits flags.
  * If file capabilities are not supported (i.e., kernels before Linux 2.6.24): grant or remove any capability in the caller's permitted capability set to or from any other process.  (This property of CAP_SETPCAP is not available when the kernel is configured to support file capabilities, since CAP_SETPCAP has entirely different semantics for such kernels.)
* CAP_SETUID
  * Make arbitrary manipulations of process UIDs (setuid(2), setreuid(2), setresuid(2), setfsuid(2));
  * forge UID when passing socket credentials via UNIX domain sockets;
  * write a user ID mapping in a user namespace (see user_namespaces(7)).
* CAP_SYS_ADMIN
  * Perform a range of system administration operations including: quotactl(2), mount(2), umount(2), swapon(2), setdomainname(2);
  * perform privileged syslog(2) operations (since Linux 2.6.37, CAP_SYSLOG should be used to permit such operations);
  * perform VM86_REQUEST_IRQ vm86(2) command;
  * perform IPC_SET and IPC_RMID operations on arbitrary System V IPC objects;
  * override RLIMIT_NPROC resource limit;
  * perform operations on trusted and security Extended Attributes (see xattr(7));
  * use lookup_dcookie(2);
  * use ioprio_set(2) to assign IOPRIO_CLASS_RT and (before Linux 2.6.25) IOPRIO_CLASS_IDLE I/O scheduling classes;
  * forge PID when passing socket credentials via UNIX domain sockets;
  * exceed /proc/sys/fs/file-max, the system-wide limit on the number of open files, in system calls that open files (e.g., accept(2), execve(2), open(2), pipe(2));
  * employ CLONE_* flags that create new namespaces with clone(2) and unshare(2) (but, since Linux 3.8, creating user namespaces does not require any capability);
  * call perf_event_open(2);
  * access privileged perf event information;
  * call setns(2) (requires CAP_SYS_ADMIN in the target namespace);
  * call fanotify_init(2);
  * call bpf(2);
  * perform privileged KEYCTL_CHOWN and KEYCTL_SETPERM keyctl(2) operations;
  * perform madvise(2) MADV_HWPOISON operation;
  * employ the TIOCSTI ioctl(2) to insert characters into the input queue of a terminal other than the caller's controlling terminal;
  * employ the obsolete nfsservctl(2) system call;
  * employ the obsolete bdflush(2) system call;
  * perform various privileged block-device ioctl(2) operations;
  * perform various privileged filesystem ioctl(2) operations;
  * perform privileged ioctl(2) operations on the /dev/random device (see random(4));
  * install a seccomp(2) filter without first having to set the no_new_privs thread attribute;
  * modify allow/deny rules for device control groups;
  * employ the ptrace(2) PTRACE_SECCOMP_GET_FILTER operation to dump tracee's seccomp filters;
  * employ the ptrace(2) PTRACE_SETOPTIONS operation to suspend the tracee's seccomp protections (i.e., the PTRACE_O_SUSPEND_SECCOMP flag);
  * perform administrative operations on many device drivers.
* CAP_SYS_BOOT
  * Use reboot(2) and kexec_load(2).
* CAP_SYS_CHROOT
  * Use chroot(2).
* CAP_SYS_MODULE
  * Load and unload kernel modules (see init_module(2) and delete_module(2));
  * in kernels before 2.6.25: drop capabilities from the system-wide capability bounding set.
* CAP_SYS_NICE
  * Raise process nice value (nice(2), setpriority(2)) and change the nice value for arbitrary processes;
  * set real-time scheduling policies for calling process, and set scheduling policies and priorities for arbitrary processes (sched_setscheduler(2), sched_setparam(2), shed_setattr(2));
  * set CPU affinity for arbitrary processes (sched_setaffinity(2));
  * set I/O scheduling class and priority for arbitrary processes (ioprio_set(2));
  * apply migrate_pages(2) to arbitrary processes and allow processes to be migrated to arbitrary nodes;
  * apply move_pages(2) to arbitrary processes;
  * use the MPOL_MF_MOVE_ALL flag with mbind(2) and move_pages(2).
* CAP_SYS_PACCT
  * Use acct(2).
* CAP_SYS_PTRACE
  * Trace arbitrary processes using ptrace(2);
  * apply get_robust_list(2) to arbitrary processes;
  * transfer data to or from the memory of arbitrary processes using process_vm_writev(2);
  * inspect processes using kcmp(2).
* CAP_SYS_RAWIO
  * Perform I/O port operations (iopl(2) and ioperm(2));
  * access /proc/kcore;
  * employ the FIBMAP ioctl(2) operation;
  * open devices for accessing x86 model-specific registers (MSRs, see msr(4));
  * update /proc/sys/vm/mmap_min_addr;
  * create memory mappings at addresses below the value specified by /proc/sys/vm/mmap_min_addr;
  * map files in /proc/bus/pci;
  * open /dev/mem and /dev/kmem;
  * perform various SCSI device commands;
  * perform certain operations on hpsa(4) and cciss(4) devices;
  * perform a range of device-specific operations on other devices.
* CAP_SYS_RESOURCE
  * Use reserved space on ext2 filesystems;
  * make ioctl(2) calls controlling ext3 journaling;
  * override disk quota limits;
  * increase resource limits (see setrlimit(2));
  * override RLIMIT_NPROC resource limit;
  * override maximum number of consoles on console allocation;
  * override maximum number of keymaps;
  * allow more than 64hz interrupts from the real-time clock;
  * raise msg_qbytes limit for a System V message queue above the limit in /proc/sys/kernel/msgmnb (see msgop(2) and msgctl(2));
  * allow the RLIMIT_NOFILE resource limit on the number of "in-flight" file descriptors to be bypassed when passing file descriptors to another process via a UNIX domain socket (see unix(7));
  * override the /proc/sys/fs/pipe-size-max limit when setting the capacity of a pipe using the F_SETPIPE_SZ fcntl(2) command.
  * use F_SETPIPE_SZ to increase the capacity of a pipe above the limit specified by /proc/sys/fs/pipe-max-size;
  * override /proc/sys/fs/mqueue/queues_max limit when creating POSIX message queues (see mq_overview(7));
  * employ the prctl(2) PR_SET_MM operation;
  * set /proc/[pid]/oom_score_adj to a value lower than the value last set by a process with CAP_SYS_RESOURCE.
* CAP_SYS_TIME
  * Set system clock (settimeofday(2), stime(2), adjtimex(2)); set real-time (hardware) clock.
* CAP_SYS_TTY_CONFIG
  * Use vhangup(2); employ various privileged ioctl(2) operations on virtual terminals.
* CAP_SYSLOG
  * Perform privileged syslog(2) operations.  See syslog(2) for information on which operations require privilege.
  * View kernel addresses exposed via /proc and other interfaces when /proc/sys/kernel/kptr_restrict has the value 1.
* CAP_WAKE_ALARM
  * Trigger something that will wake up the system (set CLOCK_REALTIME_ALARM and CLOCK_BOOTTIME_ALARM timers)