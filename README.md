# Taskie

Taskie is a console-based Task Management System written in C. It allows
users to register, log in, and manage their personal to-do list directly
from the terminal.

## Features

- User registration and login system
- Add, edit, delete, and view tasks
- Mark tasks as completed
- Automatic reset option once all tasks are completed
- Command-line login support (`taskie login <username> <password>`)
- Per-user task storage

## Project Structure

.
├── controller
│   ├── auth
│   │   ├── auth.c
│   │   └── auth.h
│   └── todo
│       ├── todo.c
│       └── todo.h
├── data
│   └── (created automatically at runtime — stores users and tasks)
├── utils
│   ├── utils.c
│   └── utils.h
├── main.c
├── Makefile
└── README.md

## Requirements

- GCC compiler (MinGW recommended on Windows)
- Windows OS (the app uses Windows-specific functions like `cls` and `_mkdir`)

## Build Instructions

make

This compiles the project and produces `taskie.exe`.

## Run Instructions

make run

or run the executable directly:

taskie.exe

## Clean Build Files

make clean

## Usage

1. Start the program.
2. Choose **Register** to create a new account, or **Login** if you already have one.
3. Once logged in, open **Taskie Manager** to:
   - Add a new task
   - View all tasks
   - Edit an existing task
   - Mark a task as completed
   - Delete a task
4. Choose **Logout** or **Exit** to close the session.

## Authors

University Project — Taskie
Student IDs: 2407093, 2407101, 2407109

## License

This project was created for academic/educational purposes.