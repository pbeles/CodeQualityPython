# Python Code Quality Tools

## Introduction


Code quality refers to the overall quality of the code. It takes into consideration things like encompassing readability, maintainability, efficiency, and adherence to best practices.

## Why do we focus on quality?

 - Code management (reducing bugs and errors)
 - Facilate collaboration with other team members
 - Easing maintenance 
 - Easing future updates 
 - Improve reliability
 - Improve software and team performance
 
## Consequences of poor code quality

 - Technical debt
 - Increased development costs
 - Decreased productivity over time

## How do we create coding standards?

 - They are agreed by a team or community
 - They chosen because a group/community agrres that they lead to more readable and maintainable code.
 
## Examples:
 - Consistent naming conventions
 - Proper code organization and modularization
 - Effective use of comments and documentation
 - Following the Don't Repeat Yourself (DRY) principle 
 - Writing testable code


## PEP - Python Enhancement Proposals

PEPs are design documents that provide information to the Python community or describe new features for Python or its processes.  PEPs serve as the announcement tools for propose new features, talk to the python, and document decisions. 

Okay, but what does that has to do with quality code?

## PEP 8: Style Guide for Python Code

PEP 8 provides coding conventions for the Python code comprising the standard library in the main Python distribution. It is one of the most popular coding standards and many projects follow PEP 8 to maintain consistency across the Python ecosystem.


### Points: 

 - Indentation: Use 4 spaces per indentation level.
 - Maximum line length: Limit lines to 79 characters for code, 72 for comments and docstrings.


Naming conventions:

 - Functions, variables, and attributes: lowercase_with_underscores
 - Classes: CapitalizedWords
 - Constants: ALL_CAPS_WITH_UNDERSCORES

Coding Structure

- Imports: Should be on separate lines and grouped (standard library, third-party, local)
- Whitespace: Use blank lines to separate functions and classes, and larger blocks of code inside functions
- Comments: Use inline comments sparingly, write docstrings for all public modules, functions, classes, and methods



## Linters and Their Importance 


A linter is a tool that analyzes source code.
It is kind of a grammarly for code.
It detects programming errors, bugs, and stylistic errors.

Linters do not **execute** the code.

Linters find:

 - Syntax errors
 - Unused variables or imports
 - Violations of coding standards
 - Potential logical errors or bugs
 - Security vulnerabilities


Why use linters?
 - Early detection of errors
 - Consitency 
 - Time saver
 - Code quality improvement
 - Integration with CI/CD
 - Help developers learn best practices and improve their coding skills

### 4. Popular Python Linters 

#### Pylint 

  ```
  pip install pylint
  ```
- Basic usage:
  ```
  pylint your_file.py
  ```

#### Black 

- Installation:
  ```
  pip install black
  ```
- Basic usage:
  ```
  black your_file.py
  ```

#### Ruff 

- Installation:
  ```
  pip install ruff
  ```
- Basic usage:
  ```
  ruff check your_file.py
  ```

### 5. Comparing Pylint, Black, and Ruff 
- Pylint: Comprehensive linter, checks style and logic
- Black: Opinionated code formatter, focuses on consistent style
- Ruff: Fast linter, combines multiple tools, customizable


### Personal take

- I always use Black and Ruff, but I only use pylint once the code is more "mature".


## Additional Resources
- [PEP 8 -- Style Guide for Python Code](https://peps.python.org/pep-0008/)
- [Pylint Documentation](https://pypi.org/project/pylint/)
- [Black Documentation](https://github.com/psf/black)
- [Ruff Documentation](https://docs.astral.sh/ruff/)
