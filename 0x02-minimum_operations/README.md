# 0x04. TypeScript

## Project Overview

This project aims to provide a foundational understanding of TypeScript by exploring various concepts such as interfaces, classes, functions, and more. By the end of this project, you'll be equipped to work with TypeScript effectively and leverage its type-checking capabilities in JavaScript applications.

## Learning Objectives

By the end of this project, you should be able to:

- Understand and utilize basic types in TypeScript.
- Define and implement interfaces and classes.
- Work with the DOM using TypeScript.
- Utilize generic types.
- Implement and use namespaces.
- Merge declarations.
- Use ambient namespaces to import external libraries.
- Apply basic nominal typing with TypeScript.

## Project Requirements

- **Editors**: vi, vim, emacs, Visual Studio Code.
- **Platform**: Ubuntu 18.04.
- **Testing**: Use Jest (version 24.9.*).
- **File Extensions**: Use `.ts` where applicable.
- **Code Quality**: The TypeScript compiler should not produce any warnings or errors.
- **Mandatory File**: A `README.md` file at the root of the project folder.

## Configuration Files

The following configuration files are provided and must be used for all tasks:

- `package.json`
- `.eslintrc.js`
- `tsconfig.json`
- `webpack.config.js`

## Tasks

### Task 0: Creating an Interface for a Student

- **Directory**: `task_0`
- **Files**: `task_0/js/main.ts`, `task_0/package.json`, `task_0/.eslintrc.js`, `task_0/tsconfig.json`, `task_0/webpack.config.js`
- **Objective**: Create a `Student` interface with `firstName`, `lastName`, `age`, and `location` fields. Render a table using Vanilla JavaScript that lists each student's `firstName` and `location`.

### Task 1: Let's Build a Teacher Interface

- **Directory**: `task_1`
- **Files**: `task_1/js/main.ts`, `task_1/webpack.config.js`, `task_1/tsconfig.json`, `task_1/package.json`
- **Objective**: Create a `Teacher` interface with attributes `firstName`, `lastName`, `fullTimeEmployee`, `yearsOfExperience` (optional), and `location`. Allow dynamic attributes (e.g., `contract`).

### Task 2: Extending the Teacher Interface

- **Directory**: `task_1`
- **Files**: `task_1/js/main.ts`
- **Objective**: Create a `Directors` interface that extends `Teacher` and includes a `numberOfReports` attribute.

### Task 3: Printing Teachers

- **Directory**: `task_1`
- **Files**: `task_1/js/main.ts`
- **Objective**: Write a function `printTeacher` that returns a formatted string with the first letter of the first name and the full last name.

### Task 4: Writing a Class

- **Directory**: `task_1`
- **Files**: `task_1/js/main.ts`
- **Objective**: Create a `StudentClass` with `firstName` and `lastName`. Implement methods `workOnHomework` and `displayName`.

### Task 5: Advanced Types Part 1

- **Directory**: `task_2`
- **Files**: `task_2/js/main.ts`, `task_2/webpack.config.js`, `task_2/tsconfig.json`, `task_2/package.json`
- **Objective**: Define `DirectorInterface` and `TeacherInterface` with specific methods. Create corresponding classes and a `createEmployee` function to instantiate either `Director` or `Teacher`.

### Task 6: Creating Functions Specific to Employees

- **Directory**: `task_2`
- **Files**: `task_2/js/main.ts`
- **Objective**: Implement functions `isDirector` and `executeWork` to differentiate between `Director` and `Teacher` based on provided arguments.

### Task 7: String Literal Types

- **Directory**: `task_2`
- **Files**: `task_2/js/main.ts`
- **Objective**: Create a string literal type `Subjects` and a function `teachClass` that returns specific strings based on the class name.

### Task 8: Ambient Namespaces

- **Directory**: `task_3`
- **Files**: `task_3/js/main.ts`, `task_3/js/interface.ts`, `task_3/js/crud.d.ts`
- **Objective**: Define types and interfaces for a mock CRUD library and use them in `main.ts` to demonstrate database operations.

### Task 9: Namespace & Declaration Merging

- **Directory**: `task_4`
- **Files**: `task_4/package.json`, `task_4/tsconfig.json`, `task_4/js/subjects/*`
- **Objective**: Create `Teacher` and `Subject` interfaces and classes using declaration merging within a namespace. Implement specific classes for `Cpp`, `Java`, and `React` with corresponding methods.

### Task 10: Update task_4/js/main.ts

- **Directory**: `task_4`
- **Files**: `task_4/js/main.ts`
- **Objective**: Create and export constants for `Cpp`, `Java`, and `React` subjects and a `Teacher` object. Log method outputs for each subject.

### Task 11: Brand Convention & Nominal Typing

- **Directory**: `task_5`
- **Files**: `task_5/js/main.ts`, `task_5/package.json`, `task_5/webpack.config.js`, `task_5/tsconfig.json`
- **Objective**: Create interfaces `MajorCredits` and `MinorCredits` with unique brand properties. Implement `sumMajorCredits` and `sumMinorCredits` functions.

## Repository Structure

- **GitHub Repository**: `alx-backend-javascript`
- **Directories**:
  - `0x04-TypeScript/task_0`
  - `0x04-TypeScript/task_1`
  - `0x04-TypeScript/task_2`
  - `0x04-TypeScript/task_3`
  - `0x04-TypeScript/task_4`
  - `0x04-TypeScript/task_5`

## Notes

- Ensure all TypeScript files compile without errors.
- Use TypeScript features effectively to enhance code quality and maintainability.

---

This README provides a high-level overview of the tasks in the 0x04 TypeScript project. For detailed implementation, refer to the provided task directories and configuration files.
