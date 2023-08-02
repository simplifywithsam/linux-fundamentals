# SSH-Keys:

## Generate SSH Key Pair (ssh-keygen):

Generate an RSA key pair: ssh-keygen
Generate an Ed25519 key pair: ssh-keygen -t ed25519
Specify a custom key file path: ssh-keygen -f /path/to/keyfile
Add a comment to the key: ssh-keygen -C "user@example.com"

## Copy Public Key to Remote Server (ssh-copy-id):

Copy the public key to the remote server: ssh-copy-id user@remote_host
Example: ssh-copy-id john@example.com

Manually Copy Public Key to Remote Server:

View the public key content: cat ~/.ssh/id_rsa.pub
Copy the public key and paste it into the remote server's ~/.ssh/authorized_keys file.

## SSH Agent (ssh-agent and ssh-add):

Start the SSH agent: eval $(ssh-agent)
Add a private key to the agent: ssh-add /path/to/private_key
List the keys added to the agent: ssh-add -l

## Disable Password Authentication (sshd_config):

Edit the SSH server configuration file: sudo nano /etc/ssh/sshd_config
Set PasswordAuthentication no

Restart the SSH service: sudo service ssh restart or sudo systemctl restart sshd


#		Example Usage:
		
		Let's use some practical examples to demonstrate the usage of these SSH key commands:
		
##		Generate SSH Key Pair (ssh-keygen):
		
		ssh-keygen: Generates an RSA key pair (id_rsa and id_rsa.pub) in the ~/.ssh/ directory.
		ssh-keygen -t ed25519: Generates an Ed25519 key pair (id_ed25519 and id_ed25519.pub) in the ~/.ssh/ directory.
		ssh-keygen -f /path/to/keyfile: Generates a key pair with a custom file path.
		ssh-keygen -C "user@example.com": Generates a key pair with a comment for identification.
		
##		Copy Public Key to Remote Server (ssh-copy-id):
		
		ssh-copy-id john@example.com: Copies the public key to the authorized_keys file on the remote server for the user "john."
		
		Manually Copy Public Key to Remote Server:
		
		cat ~/.ssh/id_rsa.pub: Views the content of the public key (for RSA keys).
		Copy the public key and paste it into the ~/.ssh/authorized_keys file on the remote server.
		
##		SSH Agent (ssh-agent and ssh-add):
		
		eval $(ssh-agent): Starts the SSH agent and sets up the environment variables.
		ssh-add /path/to/private_key: Adds a private key to the SSH agent for authentication.
		ssh-add -l: Lists the keys added to the SSH agent.
		
##		Disable Password Authentication (sshd_config):
		
		sudo nano /etc/ssh/sshd_config: Opens the SSH server configuration file for editing.
		Set PasswordAuthentication no to disable password-based authentication.
		sudo service ssh restart or sudo systemctl restart sshd: Restarts the SSH service to apply the changes.
		SSH keys provide secure and convenient authentication for remote access to servers. By following these examples and commands, you can generate SSH keys, copy them to remote servers, and configure SSH for more secure authentication mechanisms.