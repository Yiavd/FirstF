# FirstF

## How the Command works
#### What does it do?
firstf or FindFirst is a CLI tool that searches through N lines of a file and prints the lines that contains the requested pattern.
#### How run it
As previsouly mentioned, firstf runs from the terminal and requires three things:
- the pattern to search for
- the file to search in
- the number that sets the first N lines to search through in the file.
#### What commands it combines
firstf combines the grep and head commands.
- Grep is used to search a file for a pattern which then prints out the contents of the pattern.
- Head on the other hand, reads the first few lines of a file.
Combined together we get a terminal tool that allows the user to search for a pattern, like ERROR, INFO, or WARNING, within a requested number of lines (N lines) in the file. 

## AI Assisted Programming Reflection
#### What was asked?
To help make my code more efficient, I asked 5 questions to assess my firstf script being:
- What are some test cases I should use for this command?
- What edge cases could cause this program to fail?
- Why is my program not producing the expected output?
- What could cause this error in my firstf.js code?
- How can I fix this logic issue without changing the overall approach?
#### Where AI helped
AI helped me find syntax errors or bugs that I couldn't catch or comprehend. For example, one of my bugs was that one of my checks had the process.argv.length of 3, but it was meant to be 5, since we need node, firstf.js, PATTERN, FILENAME, and NUMBER_OF_LINES.
#### My own judgement
Instead of having the AI run the test cases itself, I instead ran them through my own terminal. One of the test cases was running the tool with an empty pattern argument. Since I did not implement this check, it searched and returned the requested number of lines with no specific pattern to match. After adding a check for the pattern argument, it now returns a "PATTERN is an empty string" which it didn't before.
