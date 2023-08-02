Monitoring-Tools:

System Monitor (top, htop, atop):

Display real-time system processes and resource usage: top
Interactive process viewer with dynamic updates: htop
Advanced interactive process and system resource monitoring: atop

Process Status (ps):

Show all processes running in the current terminal: ps
Show all processes running for the current user: ps -u
Show detailed information about all processes: ps aux
Show detailed information about a specific process by its PID: ps -p PID

Resource Usage (free and vmstat):

Display system memory usage: free -h
Report virtual memory statistics: vmstat

Disk Usage (df and du):

Show disk space usage of all mounted file systems: df -h
Show disk usage of a specific directory: du -h /path/to/directory

Network Monitoring (netstat and iftop):

Display all active network connections: netstat -a
Show network usage in real-time: iftop

File System Monitoring (inotifywait):

Wait for changes to files and directories: inotifywait -m /path/to/directory

Log Monitoring (tail, grep, and awk):

Display the last few lines of a log file: tail -n 20 /var/log/syslog
Search for a specific pattern in a log file: grep "ERROR" /var/log/syslog
Extract specific information from log files: awk '/pattern/ {print $2, $3}' /var/log/syslog

Performance Analysis (sar):

Collect, report, and save system activity information: sar
Generate a report for specific days or times: sar -f /var/log/sa/saXX

		Example Usage:
		
		Let's use some practical examples to demonstrate the usage of these monitoring tools commands:
		
		System Monitor (top, htop, atop):
		
		top: Displays real-time system processes and resource usage.
		htop: Provides an interactive process viewer with dynamic updates.
		atop: Offers advanced interactive process and system resource monitoring.

		Process Status (ps):
		
		ps: Shows all processes running in the current terminal.
		ps -u: Displays all processes running for the current user.
		ps aux: Shows detailed information about all processes on the system.
		ps -p 1234: Shows detailed information about the process with PID 1234.

		Resource Usage (free and vmstat):
		
		free -h: Displays system memory usage in a human-readable format.
		vmstat: Reports virtual memory statistics.

		Disk Usage (df and du):
		
		df -h: Shows disk space usage of all mounted file systems in a human-readable format.
		du -h /var/www: Shows the disk usage of the /var/www directory and its subdirectories in a human-readable format.

		Network Monitoring (netstat and iftop):
		
		netstat -a: Displays all active network connections.
		iftop: Shows network usage in real-time.

		File System Monitoring (inotifywait):
		
		inotifywait -m /path/to/directory: Monitors changes to files and directories in /path/to/directory.

		Log Monitoring (tail, grep, and awk):
		
		tail -n 20 /var/log/syslog: Displays the last 20 lines of the syslog file.
		grep "ERROR" /var/log/syslog: Searches for the word "ERROR" in the syslog file.
		awk '/pattern/ {print $2, $3}' /var/log/syslog: Extracts lines containing "pattern" and prints the second and third fields.

		Performance Analysis (sar):
		
		sar: Collects, reports, and saves system activity information.
		sar -f /var/log/sa/saXX: Generates a report for specific days or times from the sar data file.
		
		These monitoring tools help you observe system performance, resource usage, network activity, log changes, and analyze system behavior. They are crucial for maintaining system health, identifying issues, and optimizing performance.