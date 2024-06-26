# UTF-8 Validation Project

This project is designed to validate whether a given dataset represents a valid UTF-8 encoding. It requires understanding of bitwise operations, the UTF-8 encoding scheme, and proficiency in Python programming.

## Project Overview

### Objective

The main objective of this project is to implement a method that checks if a provided dataset of integers represents a valid UTF-8 encoding.

### Concepts Needed

To successfully complete this project, you'll need familiarity with the following concepts:

- **Bitwise Operations in Python:** Understanding and manipulating bits using operators like AND (&), OR (|), XOR (^), shifts (<<, >>), and bitwise NOT (~).
  
- **UTF-8 Encoding Scheme:** Knowledge of how characters are encoded into bytes, including the rules and patterns that define a valid UTF-8 sequence.

- **Data Representation:** Handling data at the byte level, particularly focusing on the 8 least significant bits (LSB) of integers.

- **List Manipulation in Python:** Iterating through lists, accessing elements, and utilizing list comprehensions effectively.

- **Boolean Logic:** Applying logical operations to make decisions within the program.

### Requirements

- **Editors:** You can use vi, vim, or emacs.
- **Execution Environment:** All files will be interpreted/compiled on Ubuntu 20.04 LTS using Python 3.4.3.
- **File Endings:** Ensure all files end with a newline.
- **Shebang Line:** The first line of all files should be `#!/usr/bin/python3`.
- **README.md:** A mandatory README.md file at the root of the project folder.
- **Coding Style:** Adhere to PEP 8 style guidelines (version 1.7.x).
- **Executable Files:** All files must be executable.

## Tasks

### Task 0: UTF-8 Validation

Implement a method `validUTF8(data)` that determines whether a given dataset `data` represents a valid UTF-8 encoding.

- **Prototype:** `def validUTF8(data)`
- **Return:** `True` if `data` is a valid UTF-8 encoding, otherwise `False`.
- **Characteristics:**
  - A UTF-8 character can span 1 to 4 bytes.
  - The dataset is represented by a list of integers where each integer represents 1 byte of data.

### Example Usage

```python
data = [65]
print(validUTF8(data))  # Output: True

data = [80, 121, 116, 104, 111, 110, 32, 105, 115, 32, 99, 111, 111, 108, 33]
print(validUTF8(data))  # Output: True

data = [229, 65, 127, 256]
print(validUTF8(data))  # Output: False
```

## Repository Information

- **GitHub Repository:** [alx-interview](https://github.com/paschalugwu/alx-interview)
- **Directory:** 0x04-utf8_validation
- **File:** 0-validate_utf8.py

## Additional Resources

- [UTF-8 Wikipedia](https://en.wikipedia.org/wiki/UTF-8)
- [The Absolute Minimum Every Software Developer Absolutely, Positively Must Know About Unicode and Character Sets](http://www.joelonsoftware.com/articles/Unicode.html)
- Mock Technical Interview (provided)
