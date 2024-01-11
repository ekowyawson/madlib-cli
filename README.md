# Lab: Class 03

## Project: File IO and Exceptions

> Author: Ekow Yawson

### Links and Resources

---

- [Python String format() Method](https://www.w3schools.com/python/ref_string_format.asp)
- [If name equals main](https://www.geeksforgeeks.org/what-does-the-if-__name__-__main__-do/)
- [Unpacking Arrays](https://realpython.com/python-kwargs-and-args/#unpacking-with-the-asterisk-operators)

### Setup

---

**Requirements:**

- Install **pytest**: run `pip3 install pytest`

**Tests:**

- To run all tests, run the following command at the root of the project:

```bash
python -m pytest

# Or, if you are in a virtual env i.e., venv:
pytest
```

### Overview

---

In this lab assignment you will be creating a command line application which takes advantage of Python’s built in capabilities for reading and writing files.

### Feature Tasks and Requirements

---

- [x] Create a file called madlib.py at root of madlib_cli folder, which will contain all of the Python code that you will write relating to your Madlib game.
- [x] Keeping in mind the concept of Single Responsibility Principle, build a command line tool which will perform the following:
  - [x] Print a welcome message to the user, explaining the `Madlib` process and command line interactions
  - [x] Read a template Madlib file (Example), and parse that file into usable parts.
  - [x] Prompt the user to submit a series of words to fit each of the required components of the Madlib template.
  - [x] With the collected user inputs, populate the template such that each provided input is placed into the correct 
        position within the template.
  - [x] After the resulting Madlib has been completed, provide the completed response back to the user in the command line.
  - [x] Write the completed text (Example)to a new file on your file system (in the repo).
  - ***Note***: A smaller example file is included as well which can be handy when developing/testing.

- **TESTING**
  - [x] Create and test a read_template function that takes in a path to text file and returns a stripped string of the file’s contents.
  - [x] The **`read_template`** should raise a `FileNotFoundError` if path is invalid.
  - [x] Create and test a `parse_template` function that takes in a template string and returns a string with language parts removed and a separate tuple of those language parts.
  - [x] Create and test a `merge` function that takes in a “**bare**” template and a list of user entered language parts,
        and returns a string with the language parts inserted into the template.
