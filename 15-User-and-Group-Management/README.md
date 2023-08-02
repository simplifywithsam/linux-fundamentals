User-and-Group-Management:

User Management:

Create a new user: sudo useradd username
Example: sudo useradd john
Set a user's password: sudo passwd username
Example: sudo passwd john
Delete a user: sudo userdel username
Example: sudo userdel john
Modify a user's information: sudo usermod options username
Example: sudo usermod -c "John Doe" john

Group Management:

Create a new group: sudo groupadd groupname
Example: sudo groupadd developers
Delete a group: sudo groupdel groupname
Example: sudo groupdel developers
Add a user to a group: sudo usermod -aG groupname username
Example: sudo usermod -aG developers john
Remove a user from a group: sudo gpasswd -d username groupname
Example: sudo gpasswd -d john developers
List groups a user belongs to: groups username
Example: groups john

Switch User (su):

Switch to another user (requires user's password): su username
Example: su john
Switch to another user with login shell: su - username
Example: su - john

		Example Usage:
		
		Let's use some practical examples to demonstrate the usage of these user and group management commands:
		
		User Management:
		
		sudo useradd john: Creates a new user named "john."
		sudo passwd john: Sets a password for the user "john."
		sudo userdel john: Deletes the user "john."
		sudo usermod -c "John Doe" john: Changes the user "john" description to "John Doe."
		
		Group Management:
		
		sudo groupadd developers: Creates a new group named "developers."
		sudo groupdel developers: Deletes the group "developers."
		sudo usermod -aG developers john: Adds the user "john" to the "developers" group.
		sudo gpasswd -d john developers: Removes the user "john" from the "developers" group.
		groups john: Shows the groups that the user "john" belongs to.
		
		Switch User (su):
		
		su john: Switches to the user "john" (requires "john"'s password).
		su - john: Switches to the user "john" with the login shell.
