Networking-Tools:

Ping (ping):

Send ICMP echo requests to a host: ping google.com
Set a specific number of packets to be sent: ping -c 5 google.com
Send packets continuously (until interrupted): ping -t google.com (Windows) or ping -i 1 google.com (Linux)

Traceroute (traceroute or tracert):

Trace the route packets take to a destination: traceroute google.com (Linux) or tracert google.com (Windows)

Network Diagnostics (nslookup or dig):

Perform DNS queries to look up IP addresses or DNS records: nslookup google.com or dig google.com

Network Scanning (nmap):

Scan for open ports on a host: nmap -p 1-1000 target_ip
Perform a TCP SYN scan: nmap -sS target_ip

Network Statistics (netstat):

Display all active network connections: netstat -a
Display listening (server) sockets: netstat -l
Display network statistics for all interfaces: netstat -i
Show the routing table: netstat -r or ip route

Transfer Data to or from a Server (curl):

Fetch data from a URL and display it in the terminal: curl https://example.com
Save the fetched data to a file: curl -o output.txt https://example.com

Securely Connect to a Remote Server (ssh):

Connect to a remote server: ssh user@remote_host
Specify a custom port for SSH: ssh -p 2222 user@remote_host
Use a specific private key for authentication: ssh -i /path/to/private_key user@remote_host

Network Interface Configuration (ifconfig or ip):

View network interface details: ifconfig or ip address
Enable a network interface: ifconfig eth0 up or ip link set eth0 up
Disable a network interface: ifconfig eth0 down or ip link set eth0 down
Assign an IP address to an interface: ifconfig eth0 192.168.1.10 or ip address add 192.168.1.10/24 dev eth0

Network Packet Capture (tcpdump or Wireshark):

Capture network packets on an interface: sudo tcpdump -i eth0
Analyze captured packets with Wireshark (GUI-based): wireshark
		
		Example Usage:
		
		Let's use some practical examples to demonstrate the usage of these networking tools commands:
		
		Ping (ping):
		
		ping google.com: Sends ICMP echo requests to the google.com server and receives echo replies.
		
		Traceroute (traceroute or tracert):
		
		traceroute google.com: Traces the route packets take to reach google.com.
		
		Network Diagnostics (nslookup or dig):
		
		nslookup google.com: Performs a DNS lookup to find the IP address of google.com.
		dig google.com: Performs a more detailed DNS query and provides additional information.
		
		Network Scanning (nmap):
		
		nmap -p 1-1000 target_ip: Scans the first 1000 ports of the target IP address.
		
		Network Statistics (netstat):
		
		netstat -a: Shows all active network connections.
		netstat -l: Displays listening (server) sockets.
		netstat -i: Shows network statistics for all interfaces.
		netstat -r: Displays the routing table.
		
		Transfer Data to or from a Server (curl):
		
		curl https://example.com: Fetches data from https://example.com and displays it in the terminal.
		curl -o output.txt https://example.com: Fetches data from https://example.com and saves it to output.txt.
		
		Securely Connect to a Remote Server (ssh):
		
		ssh user@remote_host: Establishes an SSH connection to remote_host as user.
		
		Network Interface Configuration (ifconfig or ip):
		
		ifconfig: Displays the network interface details, such as IP addresses and network configurations.
		ifconfig eth0 up: Enables the eth0 network interface.
		ifconfig eth0 down: Disables the eth0 network interface.
		ifconfig eth0 192.168.1.10: Assigns the IP address 192.168.1.10 to the eth0 interface.
		
		Network Packet Capture (tcpdump or Wireshark):
		
		sudo tcpdump -i eth0: Captures network packets on the eth0 interface.
		wireshark: Launches the Wireshark GUI to analyze captured packets.
		These networking tools are valuable for diagnosing network issues, analyzing network traffic, and managing network configurations, among other tasks. Remember to use them responsibly and with appropriate permissions, as some commands may require root privileges (sudo).