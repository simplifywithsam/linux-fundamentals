# Permissions:

## Change File Permissions (chmod):

Change permissions for a file (symbolic representation): chmod permissions file_name
Example: chmod u+rwx file.txt (Give the owner read, write, and execute permissions)
Change permissions for a file using numeric representation (octal mode): chmod 644 file.txt
Example: chmod 755 script.sh (Give read, write, and execute permissions to the owner, and read and execute permissions to group and others)

## Change File Ownership (chown):

Change the owner of a file: chown new_owner file_name
Example: chown user1 file.txt (Change the owner of file.txt to user1)
Change the owner and group of a file: chown new_owner:new_group file_name
Example: chown user1:group1 file.txt (Change the owner to user1 and the group to group1)

## Change Group Ownership (chgrp):

Change the group of a file: chgrp new_group file_name
Example: chgrp group2 file.txt (Change the group of file.txt to group2)

#		Example Usage:
		
		Let's assume we have a file named example.txt with the following permissions and ownership:
		
				-rw-r--r-- 1 user1 group1 123 Aug 2 12:34 example.txt
				
##		Change File Permissions (chmod):
		
		chmod u+x example.txt: Gives execute permission to the owner (user1) of example.txt.
		chmod go-w example.txt: Removes write permission for the group (group1) and others from example.txt.
		chmod 755 example.txt: Sets the permissions to -rwxr-xr-x, giving read, write, and execute to the owner, and read and execute to the group and others.
		
##		Change File Ownership (chown):
		
		chown user2 example.txt: Changes the owner of example.txt to user2.
		chown user2:group2 example.txt: Changes both the owner and group of example.txt to user2 and group2, respectively.
		
##		Change Group Ownership (chgrp):
		
		chgrp group3 example.txt: Changes the group of example.txt to group3.
		After applying the above commands, the file example.txt may have different permissions and ownership:
		
				-rwxr-xr-- 1 user2 group2 123 Aug 2 12:34 example.txt
				
		Always use these commands with caution, especially when changing file ownership or permissions on system-critical files. Incorrectly setting permissions or ownership may lead to system instability or security issues. Make sure you have the necessary permissions to modify the files and understand the implications of the changes you are making.
