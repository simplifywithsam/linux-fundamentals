# System-Information:

## Display System Information (uname):

Show system information: uname -a
Show the kernel name: uname -s
Show the machine hardware name: uname -m

## Display Disk Space Usage (df):

Show disk space usage of all mounted file systems: df -h
Show disk space usage of a specific directory: df -h /path/to/directory

## Display Memory Usage (free):

Show memory usage in human-readable format: free -h

## Show System Uptime (uptime):

Show how long the system has been running: uptime

## Display Logged-in Users (who):

Show who is logged on: who


#		Example Usage:
		
		Let's use some practical examples to demonstrate the usage of these system information commands:
		
##		Display System Information (uname):
		
		uname -a: Shows detailed system information, including the kernel version, architecture, and hostname.
		uname -s: Displays the kernel name.
		uname -m: Shows the machine hardware name (e.g., x86_64).
		
##		Display Disk Space Usage (df):
		
		df -h: Shows disk space usage of all mounted file systems in a human-readable format.
		df -h /home: Displays disk space usage of the /home directory.
		
##		Display Memory Usage (free):
		
		free -h: Shows memory usage (total, used, free, and swap) in a human-readable format.
		
##		Show System Uptime (uptime):
		
		uptime: Displays how long the system has been running and the average load over the last 1, 5, and 15 minutes.
		
##		Display Logged-in Users (who):
		
		who: Shows information about users who are currently logged on.
		
		Please note that the output of these commands can vary depending on the operating system and version you are using. Additionally, some commands may require administrative privileges (e.g., using sudo) to display certain information. Always double-check the commands and their options to get the most relevant system information for your needs.