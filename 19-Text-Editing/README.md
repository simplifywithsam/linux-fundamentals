Text-Editing:

Nano (nano):

Open a file for editing: nano filename
Save changes: Press Ctrl + O and then press Enter
Exit Nano: Press Ctrl + X

Vim (vim):

Open a file for editing: vim filename
Enter insert mode to start editing: Press i
Save changes and exit insert mode: Press Esc followed by :w and then press Enter
Save and quit: Press Esc followed by :wq and then press Enter
Quit without saving changes: Press Esc followed by :q! and then press Enter

Emacs (emacs):

Open a file for editing: emacs filename
Enter edit mode to start editing: Use appropriate keyboard shortcuts for specific actions.
Save changes: Press Ctrl + X, then Ctrl + S
Save and quit: Press Ctrl + X, then Ctrl + C
Quit without saving changes: Press Ctrl + X, then Ctrl + C and confirm with n

Sed (sed):

Stream Editor for text manipulation
Replace a specific word in a file: sed 's/old_word/new_word/g' filename
Example: sed 's/apples/oranges/g' fruits.txt
In-place editing of a file (modify the original file): sed -i 's/old_word/new_word/g' filename
Example: sed -i 's/apples/oranges/g' fruits.txt

Awk (awk):

Text processing tool to extract and manipulate data
Print specific columns from a file: awk '{print $1, $3}' filename
Example: awk '{print $1, $3}' data.txt
Sum values in a specific column: awk '{sum += $3} END {print sum}' filename
Example: awk '{sum += $3} END {print sum}' sales.txt

Grep (grep):

Search for a pattern in a file: grep "pattern" filename
Example: grep "error" log.txt
Search recursively in a directory and its subdirectories: grep -r "pattern" /path/to/directory
Example: grep -r "keyword" /home/user/documents
Search for a pattern case-insensitively: grep -i "pattern" filename
Example: grep -i "example" data.txt


		Example Usage:
		
		Let's use some practical examples to demonstrate the usage of these text editing commands:
		
		Nano (nano):
		
		nano example.txt: Opens the file example.txt for editing.
		While in Nano, edit the content, and then press Ctrl + O to save the changes and Ctrl + X to exit.
		
		Vim (vim):
		
		vim data.txt: Opens the file data.txt for editing.
		While in Vim, press i to enter insert mode, make changes to the content, press Esc to exit insert mode, and then type :wq to save and quit.
		
		Sed (sed):
		
		sed 's/apples/oranges/g' fruits.txt: Replaces all occurrences of "apples" with "oranges" in the file fruits.txt.
		
		Awk (awk):
		
		awk '{print $1, $3}' data.txt: Prints the first and third columns of data.txt.
		awk '{sum += $3} END {print sum}' sales.txt: Sums the values in the third column of sales.txt and prints the total.
		
		Grep (grep):
		
		grep "error" log.txt: Searches for the word "error" in the log.txt file.
		grep -r "keyword" /home/user/documents: Recursively searches for the word "keyword" in all files under the documents directory.
		These text editing commands are essential for manipulating and processing text data. They provide efficient ways to edit files, search for patterns, and extract specific information from text files.