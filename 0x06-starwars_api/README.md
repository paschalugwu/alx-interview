# Star Wars API Project

This project is focused on creating a script to fetch and display characters from the Star Wars movies using the Star Wars API. The script will accept a movie ID as a command-line argument and display the character names in the same order as they appear in the movie.

## Table of Contents

- [Introduction](#introduction)
- [Requirements](#requirements)
- [Concepts Needed](#concepts-needed)
- [Installation](#installation)
- [Usage](#usage)
- [Tasks](#tasks)
- [Additional Resources](#additional-resources)

## Introduction

The objective of this project is to interact with an external API to retrieve and display information about Star Wars characters based on a given movie ID. This involves understanding HTTP requests, working with APIs, asynchronous programming, and handling command-line arguments in Node.js.

## Requirements

- **Editors**: vi, vim, emacs
- **Environment**: Ubuntu 20.04 LTS
- **Node.js Version**: 10.14.x
- **Code Style**: Semi-standard compliant (Standard rules with semicolons)
- **File Requirements**:
  - All files should end with a new line.
  - The first line of all files should be `#!/usr/bin/node`.
  - All files must be executable.
  - No use of `var`.

## Concepts Needed

### HTTP Requests in JavaScript
- Making HTTP requests to external services using the `request` module or alternatives like `fetch` in Node.js.
- Understanding the basics of making HTTP requests, handling responses, and parsing JSON data.

### Working with APIs
- Understanding RESTful APIs and how to interact with them.
- Parsing JSON data returned by APIs to extract relevant information.

### Asynchronous Programming
- Managing asynchronous operations using callbacks, promises, and async/await syntax.
- Handling API responses asynchronously to ensure efficient data retrieval and processing.

### Command Line Arguments in Node.js
- Using the `process.argv` array to access command-line arguments passed to a Node.js script.
- Parsing and using these arguments effectively within the script.

### Array Manipulation and Iteration
- Iterating over arrays and manipulating data structures to format and display character names.
- Utilizing JavaScript array methods to handle and display data correctly.

## Installation

To set up the environment for this project, follow these steps:

1. **Install Node 10**:
    ```bash
    $ curl -sL https://deb.nodesource.com/setup_10.x | sudo -E bash -
    $ sudo apt-get install -y nodejs
    ```

2. **Install semi-standard**:
    ```bash
    $ sudo npm install semistandard --global
    ```

3. **Install the request module**:
    ```bash
    $ sudo npm install request --global
    $ export NODE_PATH=/usr/lib/node_modules
    ```

## Usage

To run the script, use the following command format:
```bash
$ ./0-starwars_characters.js <Movie ID>
```

Example:
```bash
$ ./0-starwars_characters.js 3
```

## Tasks

### 0. Star Wars Characters

Write a script that prints all characters of a Star Wars movie:

- **Input**: The first positional argument is the Movie ID (e.g., 3 for "Return of the Jedi").
- **Output**: Display one character name per line in the same order as the "characters" list in the `/films/` endpoint.
- **Requirements**:
  - Use the Star Wars API.
  - Use the `request` module.

Example output for `./0-starwars_characters.js 3`:
```text
Luke Skywalker
C-3PO
R2-D2
Darth Vader
Leia Organa
Obi-Wan Kenobi
Chewbacca
Han Solo
Jabba Desilijic Tiure
Wedge Antilles
Yoda
Palpatine
Boba Fett
Lando Calrissian
Ackbar
Mon Mothma
Arvel Crynyd
Wicket Systri Warrick
Nien Nunb
Bib Fortuna
```

## Additional Resources

For more information on the key concepts, refer to the following resources:

- [A Complete Guide to Making HTTP Requests in Node.js](https://blog.example.com/making-http-requests-in-nodejs)
- [Working with APIs in JavaScript](https://blog.example.com/working-with-apis-in-javascript)
- [Asynchronous Programming in JavaScript](https://blog.example.com/asynchronous-programming-in-javascript)
- [How to Parse Command Line Arguments in Node.js](https://blog.example.com/parse-command-line-arguments-in-nodejs)
- [JavaScript Array Methods](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)

By understanding and applying these concepts, you will be able to efficiently retrieve, process, and display Star Wars characters from the specified movie using the Star Wars API.
