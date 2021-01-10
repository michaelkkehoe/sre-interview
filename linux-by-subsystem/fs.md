# Filesystems

*Q: What are the various filesystem mount options and what do they do?*

A: They are:

* -r: Read Only
* -rw: Read Write
* -L: Label
* -U: UUID
* -t: Types (See next question)
 * async
 * atime/noatime
 * auto/ noauto
 * context
 * defaults
 * dev/ nodev
 * diraatime/ nodiratime
 * dirsync
 * exec/ noexec
 * group
 * iversion/ noiversion
 * suid/ nosuid

*Q: What are some supported filesystem types?*

A: They are:

* ADFS (Advanced Disc Filing System)
* AFFS (Aminga Fast Filesystem)
* autofs
* cifs
* coda
* coherent
* cramfs
* debugfs
* devpts
* efs
* ext
* ext2
* ext3
* ext4
* hfs
* hfsplus
* hpfs
* iso9660
* jfs
* minix
* msdos
* ncpfs
* nfs
* nfs4
* ntfs
* proc
* qnx4
* ramfs
* reiserfs
* romfs
* squashfs
* smbfs
* sysv
* tmpfs
* ubifs
* udf
* ufs
* umdos
* usbfs
* vfat
* xenix
* xfs
* xiafs

*Q: What are the basic file I/O methods?*

A: They are:

  * open()
  * read()
  * write()
  * close()

*Q: What is a file descriptor?*

A: A file descriptor is a number that uniquely identifies an open file in a computer's operating system. It describes a data resource, and how that resource may be accessed.

*Q: What are the different types of IPC?*

A:
  * Signals
  * Pipes
  * Sockets
  * File locking
  * Message Queues
  * Semaphores
  * Shared memory

*Q: What is an inode?*

A: All files (and directories) have its description stores in an inode. An inode contains the following fields

  * Device ID
  * File serial numbers
  * The file mode which determines file type and how the file owners can access the file
  * A link count telling how many hard links point to the inode
  * User ID of the file owners
  * group ID of the file
  * Device ID of the file if it's a device file
  * File size in bytes
  * Timestamps telling when the inode itself was last modified (ctime), the file content was modified (mtime) and last accessed (atime)
  * preferred I/O block size
  * The number of blocks allocated to this file

*Q: How can you speed up accessing files?*

A: Disable atime modification in /etc/fstab

*Q: What are the different types of IPC?*

A:

  * Signals
  * Pipes
  * Sockets
  * File locking
  * Message Queues
  * Semaphores
  * Shared memory

*Q: Where are filenames stored?*

A: Unix directories are what map file system names (e.g. perl) to inode numbers (e.g. 266327) that contain the actual data. A directory is a special file that the kernel maintains. Only kernel modifies directories, but processes can read directories. The contents of a directory are a list of filename and inode number pairs. When new directories are created, kernel makes two entries named '.' (refers to the directory itself) and '..' (refers to parent directory). System call for creating directory is mkdir (pathname, mode).

*Q: What is a Hard Link?*

A: Hard link is the exact replica of the actual file it is pointing to. Both the hard link and the linked file shares the same inode.

*Q: What is a Soft Link?*

A: Symbolic link (Symlinks/Soft links) are links between files. It is nothing but a shortcut of a file (in windows terms).

*Q: What is the /proc filesystem?*

A: The proc filesystem (procfs) is a special filesystem in Unix operating systems that presents information about processes and other information in a hierarchial file-like structure, providing a more convienient and standardized method for dynamically accessing process data held in the kernel. 

*Q: What is the maximum length of a filename under linux?*

A: This is based on the filesystem. Generally it’s 255 bytes for the filename

*Q:  What are filenames that are preceded by a dot?*

A: In general, filenames that are preceded by a dot are hidden files. These files can be configuration files that hold important data or setup info. Setting these files as hidden makes it less likely to be accidentally deleted.

*Q: What is a FIFO pipe?*

A: First-in-first-out pipe known as a 'named-pipe'

*Q: What is the difference between ext4 and ext3?*

A: Differences include:

  * Ext4 max file size 16TB, Ext3 is 2TB
  * Ext4 max filesystem size is 1EB, ext3  is 32TB

*Q:What Is The Difference Between Nfs Share And A Samba Share?*

A: NFS sharing is done between linux to Linux where Samba sharing can be done between Linux-Linux and Linux-windows

*Q: What Is The Command To Display All The Logical Volume Available In The System?*

A: `lvdisplay`

*Q: What is the format of a `fstab` entry?*

A: Below:

1. `fs_spec`: This field describes the block special device, remote filesystem or filesystem image for loop device to be mounted or swap file or swap partition to be enabled.
2. `fs_file`: This field describes the mount point (target) for the filesystem.
3. `fs_vfstype` Filesystem type
4. `fs_mntops` Mount Options
5. `fs_freq`: The field us used by `dump(8)` to termine which filesystems need to be dumped
6. `fs_passno`: This field is used by fsck(8) to determine the order in which filesystem checks are done at boot time .The root filesystem should be specified with a fs_passno of 1.  Other filesystems should have a fs_passno of 2.  Filesystems within a drive will be checked sequentially, but filesystems on different drives will be checked at the same time to utilize parallelism available in the hardware.  Defaults to zero (don't fsck) if not present.

*Q; What Is The Command To View All The Available Partitions On The System?*

A: fdisk -l

*Q: What is a journaling filesystem*

A: A journaling filesystem is a filesystem that maintains a special file called a journal that is used to repair any inconsistencies that occur as the result of an improper shutdown of a computer. 

*Q: What Are The Journaling Modes Supported By Ext3 Filesystem?*

A: Below:

* Ordered: Journals only metadata (This is the default)
* Journaled: Journals data as well as metadata
* Writeback: Journal updates are not atomic, but this gives better performance.

*Q: How To Kill All Actions On A Filesystem??*

A: `fuser  -km  mnt_point`

*Q: Why are partitions needed?*

A: Separate partitions improve performance by keeping data together which reduces the disk head seek.

*Q: What are the extended filesystem attributes?*

A: Extended attributes are name:value pairs associated permanently with files and directories, similar to the environment strings associated with a process.

*Q: What are common file attributes supported by many common Linux file systems?*

A:

* noatime
* append-only
* immutable
* nodump
* securedeletion
* synchronos updates

*Q: What are the extended attribute namespaces?*

A: They are:

* user
* trusted
* system
* security

*Q: Where are the extended attributes stored?*

A: Extended attributes are stored directly in inodes (on file systems with inodes bigger than 128 bytes) and on additional disk blocks. The i_file_acl field contains the block number if an inode uses an additional block. All attributes must fit in the inode and one additional block.

*Q: How do you apply quota's?*

A: https://access.redhat.com/documentation/en-us/red_hat_enterprise_linux/6/html/storage_administration_guide/ch-disk-quotas
