# FirstF

## How the Command works
#### What does it do?
firstf or FindFirst is a CLI tool that searches through N lines of a file and prints the lines that contains the requested pattern.
#### How run it
As previsouly mentioned, firstf runs from the terminal and requires three things being
- the pattern to search for
- the file to search in
- the number that sets the first N lines to search through in the file.
#### What commands it combines
firstf combines the grep and head commands.
- Grep is used to search a file for a pattern which then prints out the contents of the pattern within the file.
- Head on the other hand, head reads the first few lines of a file.
Combined together we get a terminal tool that allows the user to search for a pattern, like ERROR, INFO, or WARNING, within a requested number of lines (N lines) in the file. 

## AI Assisted Programming Reflection
