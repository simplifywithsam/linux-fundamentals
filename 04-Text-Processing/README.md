Text-Processing:

Search for Patterns in Files (grep):

Search for a word in a file: grep "word" myfile.txt
Search for a word case-insensitively: grep -i "word" myfile.txt
Search for a word recursively in a directory: grep -r "word" /path/to/directory
Search for a pattern using a regular expression: grep -E "pattern" myfile.txt

Stream Editor for Text Manipulation (sed):

Replace text in a file: sed 's/old_text/new_text/' myfile.txt
Replace text in a file and save the changes in-place: sed -i 's/old_text/new_text/' myfile.txt
Delete lines matching a pattern: sed '/pattern/d' myfile.txt
Print only specific lines: sed -n '5,10p' myfile.txt

Text Processing and Pattern Matching Tool (awk):

Print specific columns from a file: awk '{print $1, $3}' myfile.txt
Calculate the sum of values in a specific column: awk '{sum += $2} END {print sum}' myfile.txt
Filter lines based on a condition: awk '$2 > 50 {print}' myfile.txt

		Example Usage:
		
		Let's assume we have the following file named myfile.txt:
		
		
		1. Alice: 25
		2. Bob: 30
		3. Carol: 20
		4. David: 40
		5. Eve: 50
		
		
		Search for Patterns in Files (grep):
		
		grep "Bob" myfile.txt: Searches for the word "Bob" in myfile.txt and outputs the line containing it.
		grep -i "alice" myfile.txt: Searches case-insensitively for the word "alice" in myfile.txt.
		grep -r "David" /path/to/directory: Recursively searches for the word "David" in all files under the specified directory.
		grep -E "A|E" myfile.txt: Searches for lines containing either "A" or "E" using a regular expression.
		
		Stream Editor for Text Manipulation (sed):
		
		sed 's/Carol/Caroline/' myfile.txt: Replaces "Carol" with "Caroline" in myfile.txt without changing the file.
		sed -i 's/Bob/Robert/' myfile.txt: Replaces "Bob" with "Robert" in myfile.txt and saves the changes in-place.
		sed '/Alice/d' myfile.txt: Deletes lines containing the word "Alice" from myfile.txt.
		sed -n '2,4p' myfile.txt: Prints lines 2 to 4 from myfile.txt (Bob, Carol, and David).
		
		Text Processing and Pattern Matching Tool (awk):
		
		awk '{print $1, $3}' myfile.txt: Prints the first and third columns (names and ages) from myfile.txt.
		awk '{sum += $2} END {print sum}' myfile.txt: Calculates and prints the sum of ages from the second column in myfile.txt.
		awk '$2 > 25 {print}' myfile.txt: Prints lines where the value in the second column (ages) is greater than 25.
		
		These text processing commands are powerful tools for searching, manipulating, and extracting information from text files. You can combine them with other Linux commands to perform more complex operations and data analysis on text data. Always ensure that you carefully construct your patterns and conditions to achieve the desired results.
