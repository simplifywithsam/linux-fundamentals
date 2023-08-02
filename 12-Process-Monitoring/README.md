Process-Monitoring:

Display Running Processes (ps):

Show all processes running in the current terminal: ps
Show all processes running for the current user: ps -u
Show detailed information about all processes: ps aux
Show detailed information about a specific process by its PID: ps -p PID

Monitor Real-Time System Processes (top):

View real-time process activity: top
Sort processes by CPU usage: Press Shift + P
Sort processes by memory usage: Press Shift + M
Search for a specific user's processes: Press u and enter the username

Dynamic Real-Time Process Monitoring (htop):

Monitor system processes interactively with a dynamic interface: htop

View Process Tree (pstree):

Display a tree-like representation of running processes: pstree
Show process tree for a specific process by its PID: pstree -p PID

Track Process Activity (strace):

Monitor system calls made by a process: strace -p PID

Monitor Process Resource Usage (top, htop, atop):

Continuously monitor resource usage for all processes: top
Monitor resource usage for a specific process by its PID: top -p PID
Monitor resource usage interactively with htop: htop
Advanced interactive process monitoring with atop: atop


		Example Usage:
		
		Let's use some practical examples to demonstrate the usage of these process monitoring commands:
		
		Display Running Processes (ps):
		
		ps: Displays a list of processes running in the current terminal session.
		ps -u: Shows all processes running for the current user.
		ps aux: Displays detailed information about all processes on the system.
		ps -p 1234: Shows detailed information about the process with PID 1234.
		
		Monitor Real-Time System Processes (top):
		
		top: Displays real-time system statistics and a list of active processes.
		While in top, pressing Shift + P sorts the processes by CPU usage.
		While in top, pressing Shift + M sorts the processes by memory usage.
		While in top, pressing u and entering the username filters the processes by that specific user.
		
		Dynamic Real-Time Process Monitoring (htop):
		
		htop: Launches an interactive process viewer with dynamic updates.
		
		View Process Tree (pstree):
		
		pstree: Displays a tree-like representation of running processes.
		
		Track Process Activity (strace):
		
		strace -p 1234: Monitors the system calls made by the process with PID 1234.
		
		Monitor Process Resource Usage (top, htop, atop):
		
		top: Continuously monitors resource usage for all processes.
		top -p 1234: Monitors resource usage for the process with PID 1234.
		htop: Provides an interactive resource usage view with dynamic updates.
		atop: Provides advanced interactive process and system resource monitoring.
		
		These process monitoring commands are essential for observing and understanding the behavior of running processes, tracking resource usage, and troubleshooting performance issues on a system. Use them to identify resource-hungry processes, analyze system activity, and optimize system performance.