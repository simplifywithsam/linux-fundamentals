# Networking:

## Ping (ping):

Send ICMP echo requests to a host: ping google.com
Set a specific number of packets to be sent: ping -c 5 google.com
Send packets continuously (until interrupted): ping -t google.com (Windows) or ping -i 1 google.com (Linux)

## Configure Network Interfaces (ifconfig or ip):

View network interface details: ifconfig or ip address
Enable a network interface: ifconfig eth0 up or ip link set eth0 up
Disable a network interface: ifconfig eth0 down or ip link set eth0 down
Assign an IP address to an interface: ifconfig eth0 192.168.1.10 or ip address add 192.168.1.10/24 dev eth0

## Display Network Statistics (netstat):

Display all active network connections: netstat -a
Display listening (server) sockets: netstat -l
Display network statistics for all interfaces: netstat -i
Show the routing table: netstat -r or ip route

## Securely Connect to a Remote Server (ssh):

Connect to a remote server: ssh user@remote_host
Specify a custom port for SSH: ssh -p 2222 user@remote_host
Use a specific private key for authentication: ssh -i /path/to/private_key user@remote_host

## Copy Files Between Local and Remote Systems (scp):

Copy a file from local to remote: scp local_file.txt user@remote_host:/path/to/destination/
Copy a file from remote to local: scp user@remote_host:/remote_path/remote_file.txt /local_path/

## Transfer Data to or from a Server (curl):

Fetch data from a URL and display it in the terminal: curl https://example.com
Save the fetched data to a file: curl -o output.txt https://example.com


#		Example Usage:
		
		Let's use some practical examples to demonstrate the usage of these networking commands:
		
##		Ping (ping):
		
		ping google.com: Sends ICMP echo requests to the google.com server and receives echo replies.
		
##		Configure Network Interfaces (ifconfig or ip):
		
		ifconfig: Displays the network interface details, such as IP addresses and network configurations.
		ifconfig eth0 up: Enables the eth0 network interface.
		ifconfig eth0 down: Disables the eth0 network interface.
		ifconfig eth0 192.168.1.10: Assigns the IP address 192.168.1.10 to the eth0 interface.
		
##		Display Network Statistics (netstat):
		
		netstat -a: Shows all active network connections.
		netstat -l: Displays listening (server) sockets.
		netstat -i: Shows network statistics for all interfaces.
		netstat -r: Displays the routing table.
		
##		Securely Connect to a Remote Server (ssh):
		
		ssh user@remote_host: Establishes an SSH connection to remote_host as user.
		
##		Copy Files Between Local and Remote Systems (scp):
		
		scp local_file.txt user@remote_host:/path/to/destination/: Copies local_file.txt from the local system to remote_host under /path/to/destination/.
		
##		Transfer Data to or from a Server (curl):
		
		curl https://example.com: Fetches data from https://example.com and displays it in the terminal.
		curl -o output.txt https://example.com: Fetches data from https://example.com and saves it to output.txt.
		
		These networking commands are essential for managing network connections, transferring files, and troubleshooting network-related issues. Use them with appropriate options and parameters as needed for your specific use cases.
