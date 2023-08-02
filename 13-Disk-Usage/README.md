# Disk-Usage:

## Display Disk Space Usage (df):

Show disk space usage of all mounted file systems: df -h
Show disk space usage of a specific directory: df -h /path/to/directory

## Display Directory Disk Usage (du):

Show the disk usage of a directory and its subdirectories: du -h /path/to/directory
Show only the total disk usage of a directory: du -sh /path/to/directory
Show disk usage in human-readable format (e.g., MB, GB): du -h /path/to/directory

## Find Large Files or Directories (find and du combination):

Find the top N largest files in a directory: find /path/to/directory -type f -exec du -h {} + | sort -rh | head -n N
Example: find /home/user -type f -exec du -h {} + | sort -rh | head -n 5 (Finds the 5 largest files in the /home/user directory)

#		Example Usage:
		
		Let's use some practical examples to demonstrate the usage of these disk usage commands:
		
## 		Display Disk Space Usage (df):
		
		df -h: Shows disk space usage of all mounted file systems in a human-readable format.
		df -h /home: Displays disk space usage of the /home directory.
		
## 		Display Directory Disk Usage (du):
		
		du -h /var/www: Shows the disk usage of the /var/www directory and its subdirectories in a human-readable format.
		du -sh /home/user: Shows only the total disk usage of the /home/user directory in a human-readable format.
		du -h /opt: Shows the disk usage of the /opt directory and its subdirectories in human-readable format.
		
## 		Find Large Files or Directories (find and du combination):
		
		find /var/log -type f -exec du -h {} + | sort -rh | head -n 10: Finds the 10 largest files in the /var/log directory.
		find /home/user/docs -type f -exec du -h {} + | sort -rh | head -n 5: Finds the 5 largest files in the /home/user/docs directory.
