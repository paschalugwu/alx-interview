## Project: 0x03. Log Parsing

### Description
This project focuses on parsing and processing data streams in real-time using Python programming. The main goal is to read from standard input (stdin), handle data in a specific format, and perform calculations based on the input data.

### Concepts Needed
1. **File I/O in Python**:
   - Reading from `sys.stdin` line by line.
   - Python Input and Output

2. **Signal Handling in Python**:
   - Handling keyboard interruption (CTRL + C) using signal handling in Python.
   - Python Signal Handling

3. **Data Processing**:
   - Parsing strings to extract specific data points.
   - Aggregating data to compute summaries.

4. **Regular Expressions**:
   - Using regular expressions to validate the format of each line.
   - Python Regular Expressions

5. **Dictionaries in Python**:
   - Using dictionaries to count occurrences of status codes and accumulate file sizes.
   - Python Dictionaries

6. **Exception Handling**:
   - Handling possible exceptions during file reading and data processing.
   - Python Exceptions

### Tasks
#### 0. Log parsing
- Write a script that reads `stdin` line by line and computes metrics based on the input format.
- After every 10 lines or a keyboard interruption (`CTRL + C`), print statistics including total file size and number of lines by status code.

### Requirements
- Allowed editors: `vi`, `vim`, `emacs`
- Interpreted/compiled on Ubuntu 20.04 LTS using `python3` (version 3.4.3)
- Follow `PEP 8` style guidelines
- All files must be executable
- Include a `README.md` file at the root of the project folder

### Additional Resources
- Mock Technical Interview

### Repository Information
- GitHub repository: `alx-interview`
- Directory: `0x03-log_parsing`
- File: `0-stats.py`

For detailed instructions and implementation, refer to the project guidelines and resources provided. Good luck with your log parsing project!
