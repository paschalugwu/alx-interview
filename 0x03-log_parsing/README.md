# 0x03. Log Parsing

## Project Overview

This project, **0x03. Log Parsing**, is part of the ALX curriculum, focusing on parsing and processing data streams in real-time using Python. The goal is to read log data from standard input, handle it efficiently, and compute specific metrics.

## Concepts and Skills

To complete this project, you need to be proficient in the following areas:

- **File I/O in Python**: Reading from `sys.stdin` line by line.
- **Signal Handling in Python**: Handling keyboard interruptions (CTRL + C).
- **Data Processing**: Parsing strings to extract data points and aggregating data.
- **Regular Expressions**: Validating the format of log lines.
- **Dictionaries in Python**: Counting occurrences and accumulating data.
- **Exception Handling**: Managing potential exceptions during file reading and processing.

## Project Requirements

- **Editors**: vi, vim, emacs
- **Environment**: Ubuntu 20.04 LTS with Python 3.4.3
- **Code Style**: PEP 8 (version 1.7.x)
- **Executable Files**: All scripts must be executable
- **File Format**: Each file should end with a new line and start with `#!/usr/bin/python3`

## Task Description

### Task 0: Log Parsing

**Objective**: Write a Python script that reads log entries from stdin, processes them, and prints computed metrics.

#### Input Format

```
<IP Address> - [<date>] "GET /projects/260 HTTP/1.1" <status code> <file size>
```

If a line doesn't match this format, it should be skipped.

#### Output

After every 10 lines and/or on a keyboard interruption (CTRL + C), print the following statistics:

- **Total file size**: Sum of all `<file size>` values.
- **Number of lines by status code**:
  - Status codes: 200, 301, 400, 401, 403, 404, 405, 500
  - Format: `<status code>: <number>`
  - Print status codes in ascending order

#### Example

```sh
alexa@ubuntu:~/0x03-log_parsing$ ./0-generator.py | ./0-stats.py 
File size: 5213
200: 2
401: 1
403: 2
404: 1
405: 1
500: 3
File size: 11320
200: 3
301: 2
400: 1
401: 2
403: 3
404: 4
405: 2
500: 3
...
^CFile size: 17146
200: 4
301: 3
400: 4
401: 2
403: 6
404: 6
405: 4
500: 4
```

#### Implementation Guidelines

1. **Reading Input**: Continuously read lines from stdin.
2. **Parsing and Validation**: Use regular expressions to validate and extract data.
3. **Data Aggregation**: Use dictionaries to count status codes and accumulate file sizes.
4. **Printing Statistics**: Output aggregated data every 10 lines or on keyboard interruption.
5. **Exception Handling**: Ensure the program handles unexpected input and interruptions gracefully.

## Repository

- **GitHub Repository**: [alx-interview](https://github.com/alx-interview)
- **Directory**: `0x03-log_parsing`
- **File**: `0-stats.py`

## Additional Resources

- [Python Input and Output](https://docs.python.org/3/tutorial/inputoutput.html)
- [Python Signal Handling](https://docs.python.org/3/library/signal.html)
- [Python Regular Expressions](https://docs.python.org/3/library/re.html)
- [Python Dictionaries](https://docs.python.org/3/tutorial/datastructures.html#dictionaries)
- [Python Exceptions](https://docs.python.org/3/tutorial/errors.html)

By mastering these concepts and following the guidelines, you will be able to efficiently handle log parsing and data processing in Python.
