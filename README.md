TWASI – Tiny Weirdly Awesome Script Interpreter 

TWASI is a lightweight, interactive scripting interpreter written in Python.
It allows users to write and execute simple custom scripts using a minimal, beginner-friendly syntax.

The project was created as an educational experiment to explore how interpreters work internally and how custom scripting languages can be built on top of Python.

Features

Interactive IDE-like mode in terminal

Custom commands:
```
show() – print output

rand(a, b) – generate random integer

wait(seconds) – pause execution

input() – user input

randlist(list) – random choice from list

clr() – clear console
```
Variable assignment using name: value

Basic conditional logic (if / else)

Delayed execution with /run command

How It Works

The interpreter:

Collects user input line by line

Stores commands internally

Executes all stored commands when /run is entered

Supports simple IF/ELSE block execution

Uses Python’s exec() and eval() to process expressions dynamically

Installation

Clone the repository:
```
git clone https://github.com/towasi-dot/twasi.git
cd twasi
```

Run the interpreter:
```
python TWasi.py
```
Example Usage
```
x: rand(1, 10)

if x > 5 (
    show("Big number!")
)
else (
    show("Small number!")
)

/run
```

Syntax Overview
Variable Assignment
name: expression


Example:
```
score: 10
```
Printing Output
```
show("Hello World")
```
Conditional Blocks
```
if condition (
    commands
)
else (
    commands
)
```
Limitations

No support for nested conditionals

No loops

No user-defined functions

Uses eval() and exec() (not secure for untrusted input)

Minimal syntax validation

This project is intended for experimentation and learning purposes only.

Educational Purpose

TWASI is designed to help understand:

How interpreters collect and execute commands

How dynamic execution works in Python

Basic parsing logic

Control flow implementation

It is not intended for production use.
