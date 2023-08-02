# Process-Management:

## Display Information about Running Processes (ps):

Show all processes running in the current terminal: ps
Show all processes running for the current user: ps -u
Show detailed information about all processes: ps aux
Show detailed information about a specific process by its PID (Process ID): ps -p PID

## Monitor Real-Time System Processes (top):

View real-time process activity: top
Sort processes by CPU usage: Press Shift + P
Sort processes by memory usage: Press Shift + M
Search for a specific user's processes: Press u and enter the username

## Terminate Processes (kill):

Terminate a process by its PID: kill PID
Send a SIGKILL signal to forcefully terminate a process: kill -9 PID
Terminate a process by its name: killall process_name
Send a SIGKILL signal to forcefully terminate a process by its name: killall -9 process_name


#		Example Usage:
		
		Let's use some practical examples to demonstrate the usage of these process management commands:
		
##		Display Information about Running Processes (ps):
		
		ps: Displays a list of processes running in the current terminal session.
		ps -u: Shows all processes running for the current user.
		ps aux: Displays detailed information about all processes on the system.
		ps -p 1234: Shows detailed information about the process with PID 1234.
		
##		Monitor Real-Time System Processes (top):
		
		top: Displays real-time system statistics and a list of active processes.
		While in top, pressing Shift + P sorts the processes by CPU usage.
		While in top, pressing Shift + M sorts the processes by memory usage.
		While in top, pressing u and entering the username filters the processes by that specific user.
		
##		Terminate Processes (kill):
		
		kill 1234: Sends a termination signal to the process with PID 1234 to gracefully terminate it.
		kill -9 5678: Sends a SIGKILL signal to the process with PID 5678 to forcefully terminate it.
		killall firefox: Terminates all processes with the name "firefox."
		killall -9 chrome: Sends a SIGKILL signal to forcefully terminate all processes with the name "chrome."
		
		Remember to exercise caution when terminating processes, especially with the kill -9 command, as it forcefully terminates the process without allowing it to clean up or save data. Always double-check the PID or process name before sending termination signals to avoid unintended consequences.