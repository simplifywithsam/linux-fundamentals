All data in Unix is organized into files. All files are organized into directories. These directories are organized into a tree-like structure called the filesystem.

When you work with Unix, one way or another, you spend most of your time working with files. This tutorial will help you understand how to create and remove files, copy and rename them, create links to them, etc.

In Unix, there are three basic types of files −

	Ordinary Files − An ordinary file is a file on the system that contains data, text, or program instructions. In this tutorial, you look at working with ordinary files.

	Directories − Directories store both special and ordinary files. For users familiar with Windows or Mac OS, Unix directories are equivalent to folders.

	Special Files − Some special files provide access to hardware such as hard drives, CD-ROM drives, modems, and Ethernet adapters. Other special files are similar to aliases or shortcuts and enable you to access a single file using different names.

Listing Files
To list the files and directories stored in the current directory, use the following command −

$ls
Here is the sample output of the above command −

		$ls
		
		bin        hosts  lib     res.03
		ch07       hw1    pub     test_results
		ch07.bak   hw2    res.01  users
		docs       hw3    res.02  work
		The command ls supports the -l option which would help you to get more information about the listed files −

		$ls -l
		total 1962188
		
		drwxrwxr-x  2 amrood amrood      4096 Dec 25 09:59 uml
		-rw-rw-r--  1 amrood amrood      5341 Dec 25 08:38 uml.jpg
		drwxr-xr-x  2 amrood amrood      4096 Feb 15  2006 univ
		drwxr-xr-x  2 root   root        4096 Dec  9  2007 urlspedia
		-rw-r--r--  1 root   root      276480 Dec  9  2007 urlspedia.tar
		drwxr-xr-x  8 root   root        4096 Nov 25  2007 usr
		drwxr-xr-x  2    200    300      4096 Nov 25  2007 webthumb-1.01
		-rwxr-xr-x  1 root   root        3192 Nov 25  2007 webthumb.php
		-rw-rw-r--  1 amrood amrood     20480 Nov 25  2007 webthumb.tar
		-rw-rw-r--  1 amrood amrood      5654 Aug  9  2007 yourfile.mid
		-rw-rw-r--  1 amrood amrood    166255 Aug  9  2007 yourfile.swf
		drwxr-xr-x 11 amrood amrood      4096 May 29  2007 zlib-1.2.3
