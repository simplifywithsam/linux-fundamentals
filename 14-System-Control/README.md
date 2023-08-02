System-Control:

System control commands can have different implementations and utilities based on the operating system and the init system used. Below are some common system control commands along with examples for Linux systems using the systemd init system:

Start, Stop, and Restart Services (systemctl):

Start a service: sudo systemctl start service_name
Example: sudo systemctl start apache2 (Starts the Apache web server)
Stop a service: sudo systemctl stop service_name
Example: sudo systemctl stop apache2 (Stops the Apache web server)
Restart a service: sudo systemctl restart service_name
Example: sudo systemctl restart nginx (Restarts the Nginx web server)

Enable or Disable Services at Boot (systemctl):

Enable a service to start at boot: sudo systemctl enable service_name
Example: sudo systemctl enable sshd (Enables the SSH server to start at boot)
Disable a service from starting at boot: sudo systemctl disable service_name
Example: sudo systemctl disable postfix (Disables the Postfix mail server from starting at boot)

View Service Status (systemctl):

Check the status of a service: systemctl status service_name
Example: systemctl status mysql (Shows the status of the MySQL database server)
Display a list of all services: systemctl list-units --type=service

Reboot and Shutdown (systemctl):

Reboot the system: sudo systemctl reboot
Shutdown the system: sudo systemctl poweroff

Suspend and Hibernate (systemctl):

Suspend the system: sudo systemctl suspend
Hibernate the system: sudo systemctl hibernate

		Example Usage:
		
		Let's use some practical examples to demonstrate the usage of these system control commands:
		
		Start, Stop, and Restart Services (systemctl):
		
		sudo systemctl start nginx: Starts the Nginx web server.
		sudo systemctl stop apache2: Stops the Apache web server.
		sudo systemctl restart sshd: Restarts the SSH server.
		
		Enable or Disable Services at Boot (systemctl):
		
		sudo systemctl enable postgresql: Enables the PostgreSQL database server to start at boot.
		sudo systemctl disable sendmail: Disables the Sendmail mail server from starting at boot.
		
		View Service Status (systemctl):
		
		systemctl status mysql: Shows the status of the MySQL database server.
		systemctl list-units --type=service: Displays a list of all services and their current states.
		
		Reboot and Shutdown (systemctl):
		
		sudo systemctl reboot: Reboots the system.
		sudo systemctl poweroff: Shuts down the system.
		
		Suspend and Hibernate (systemctl):
		
		sudo systemctl suspend: Puts the system into a suspended state.
		sudo systemctl hibernate: Puts the system into hibernation.