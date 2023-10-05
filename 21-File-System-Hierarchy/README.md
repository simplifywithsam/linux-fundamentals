# File System Hierarchy

The File System Hierarchy Standard (FHS) is a set of conventions and guidelines for organizing the file system structure on Unix-like operating systems, including Linux. FHS defines a standardized directory structure to ensure consistency and compatibility among different Linux distributions and Unix-like systems. This standard helps users and system administrators locate and manage files and directories in a predictable manner. Here is an overview of the primary directories defined by the FHS:

## / (Root Directory):

The root directory is the top-level directory in the file system hierarchy.
It contains all other directories and files on the system.
Typically, only the root user has write access to this directory.

## /bin (Essential User Binaries):

Contains essential binary executables and commands required for system recovery and maintenance, even if no other file systems are mounted.
Examples include commands like ls, cp, mv, rm, and cat.

## /boot (Boot Files):

Contains files and boot loader configuration needed for booting the operating system.
Kernel images, bootloader files (e.g., GRUB configuration), and initial ramdisk (initrd) files are stored here.

## /dev (Device Files):

Contains special files representing devices (hardware and virtual) on the system.
Device files are used to access and interact with hardware devices, such as disk drives, terminals, and printers.

## /etc (Configuration Files):

Contains system-wide configuration files and scripts.
Configuration files for various software packages and system services are stored here.

## /home (User Home Directories):

Contains home directories for regular users.
Each user has a subdirectory here, typically named after their username, where they can store personal files and configuration settings.

## /lib and /lib64 (Library Files):

/lib stores essential shared libraries and kernel modules needed for system boot and recovery.
/lib64 is used for 64-bit libraries on 64-bit systems.

## /media and /mnt (Removable Media and Mount Points):

/media is often used for mounting removable media such as USB drives and optical discs.
/mnt is traditionally used for manually mounted file systems.

## /opt (Optional Software Packages):

Contains subdirectories for optional software packages that are not part of the core system distribution.
Some software vendors install their applications in /opt.

## /sbin (System Binaries):

Contains system administration executables, typically used by the root user.
Commands in /sbin are critical for system maintenance and repair.

## /srv (Service Data):

Contains data for services provided by the system.
Typically used for storing data associated with web servers, FTP servers, and other network services.

## /tmp (Temporary Files):

Contains temporary files created by applications and users.
Files in /tmp may be deleted automatically when the system reboots.

## /usr (User Binaries and Libraries):

Contains user-accessible programs, libraries, and documentation.
Often mounted as a separate file system to facilitate sharing among multiple machines.

## /var (Variable Data):

Contains variable data files, including log files, spool directories, and temporary files created by system processes.
It's common to mount /var on a separate partition to prevent it from filling up the root file system.

The File System Hierarchy Standard helps maintain consistency and allows Linux distributions to provide a common base structure while accommodating variations and additional directories specific to their needs. Understanding this hierarchy is essential for managing files and directories in Linux effectively.