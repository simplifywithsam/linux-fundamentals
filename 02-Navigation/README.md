**Navigation:**
		
Change Directory (cd):

Change to the home directory: cd ~
Change to a specific directory: cd /path/to/directory
Go back to the previous directory: cd ..
Go to the parent directory: cd ../..
Change to the previous directory (shortcut): cd -


List Files and Directories (ls):

List files and directories in the current directory: ls
List files and directories in a specific directory: ls /path/to/directory
List all files (including hidden files): ls -a
List files with detailed information: ls -l
List files in a human-readable format: ls -lh


Print Working Directory (pwd):

Display the current working directory: pwd


Create a New Directory (mkdir):

Create a new directory in the current location: mkdir new_directory
Create a nested directory: mkdir -p parent_directory/child_directory


Remove a Directory (rmdir):

Remove an empty directory: rmdir empty_directory


		Example Usage:
		
		Let's assume we have the following directory structure:
		
		/home/user
			├── documents
			│   ├── file1.txt
			│   ├── file2.txt
			│   └── file3.txt
			└── projects
				├── project1
				└── project2
		
		Change Directory (cd):
		
		cd /home/user/documents: Changes the current directory to /home/user/documents.
		cd ..: Goes back to the parent directory /home/user.
		cd ~/projects: Changes to the directory /home/user/projects.
		cd -: Switches back to the previous directory, /home/user.
		
		List Files and Directories (ls):
		
		ls: Lists the files and directories in the current directory (documents and projects).
		ls /home/user/documents: Lists the files in the documents directory (file1.txt, file2.txt, and file3.txt).
		ls -a: Lists all files and directories, including hidden files (e.g., .bashrc).
		ls -l: Lists files with detailed information (permissions, owner, group, size, modification date, etc.).
		ls -lh: Lists files with detailed information in a human-readable format (e.g., sizes in KB, MB, etc.).
		
		Print Working Directory (pwd):
		
		pwd: Displays the current working directory (e.g., /home/user).
		
		Create a New Directory (mkdir):
		
		mkdir new_folder: Creates a new directory named new_folder in the current location.
		mkdir -p /home/user/projects/project3: Creates the nested directory project3 inside projects, even if projects does not exist.
		
		Remove a Directory (rmdir):

		rmdir new_folder: Removes the empty directory new_folder from the current location.
		Please note that the rmdir command can only remove empty directories. If you want to remove directories with content, you can use the rm command with the -r or -rf option, but be cautious as it can lead to data loss if used incorrectly. Always double-check the directory you are deleting to avoid unintended consequences.
