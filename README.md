# alx-low_level_programming

# Shell Project
This project is a simple UNIX command-line interpreter, also known as a shell. It is capable of reading commands from standard input, parsing them, and executing them.

## 0x16. C - Simple Shell

### Pre-requisites

#### Authorized functions and macros:
- access (man 2 access)
- chdir (man 2 chdir)
- close (man 2 close)
- closedir (man 3 closedir)
- execve (man 2 execve)
- exit (man 3 exit)
- _exit (man 2 _exit)
- fflush (man 3 fflush)
- fork (man 2 fork)
- free (man 3 free)
- getcwd (man 3 getcwd)
- getline (man 3 getline)
- isatty (man 3 isatty)
- kill (man 2 kill)
- malloc (man 3 malloc)
- open (man 2 open)
- opendir (man 3 opendir)
- perror (man 3 perror)
- read (man 2 read)
- readdir (man 3 readdir)
- signal (man 2 signal)
- stat (__xstat) (man 2 stat)
- lstat (__lxstat) (man 2 lstat)
- fstat (__fxstat) (man 2 fstat)
- strtok (man 3 strtok)
- wait (man 2 wait)
- waitpid (man 2 waitpid)
- wait3 (man 2 wait3)
- wait4 (man 2 wait4)
- write (man 2 write)


## Project Structure

The project is organized as follows:




 file lists the contributors to the project. 

 file you are currently reading is a brief overview of the project. 

 file is the man page for the shell.

: a header file that includes all the necessary libraries, function prototypes, and global variables.

: the main file that contains the loop for getting the user input, parsing the input, and executing the command.

: a file that handles the prompt display for the shell.

: a file that contains the functions for executing the non-built-in commands.

 : This file contains the implementation of functions for parsing user input into arguments.

: This file contains the implementation of functions for deallocating memory.

: This file contains the implementation of signal handler functions for handling SIGINT, SIGTSTP and SIGQUIT signals.

: These are the source code files that contains functions related to the implementations of the built-in commands (cd, exit, env, setenv, unsetenv and help).

: These are the source code files that contains functions related to working with the system's PATH environment variable, such as finding a command in the PATH, getting the current PATH, and setting or modifying the PATH.

: a file that contains utility functions for the shell, such as string manipulation functions and functions for printing error messages.

: This file contains the implementation of functions for handling errors.

: a file that specifies the compilation rules for the shell.

: These are test files for each of the implementation files in source_files. 

This tree separates the implementation files from the test files, making it easier to navigate the project and run the tests.

## Function Prototypes.

The header file declares several function prototypes for the shell program, including:

: prints the shell prompt

: executes a command with arguments

: Read input from the standard input. Custom getline().

: Retrieves user input from stdin. Uses getline().

: parsing user input into arguments.

: signal handler for SIGINT

: signal handler for SIGSTP

: signal handler for SIGQUIT

: checks if a command is a shell builtin

: prints environment variables

: sets an environment variable

: unsets an environment variable

: prints help information for the shell

: changes the current working directory

: exits the shell program with a status code

: retrieves the value of an environment variable

: searches for a command in the directories specified by the PATH environment variable

: retrieves the PATH environment variable

: sets the PATH environment variable

: appends a directory to the PATH environment variable

: prepends a directory to the PATH environment variable

: frees memory allocated following system error

: frees memory allocated for tokens

: prints an error message

: prints a string

: converts a string to an integer

: prints a character

: gets the length of a string

: compares two strings

: copies a string

: concatenates two strings

: duplicates a string

: searches a string for a character

: searches for the first occurrence of a substring

: gets the length of a prefix substring

## Usage

To use the simple shell, compile the files using . Then, run the shell using .



This wil compile all the '.c' files and change the output's name to 'hsh'.

### Template to test output:
=============


also in non-interactive mode:


## Man Page.

To generate a man page for the , you can use the  utility.  allows you to write man pages in Markdown format and then convert them to man page format.

Once you have created the  file, run the following command to generate the man page:



This will create a new file called . You can view the man page by running the following command:



## AUTHORS

This program was written by 'Mhleli07'.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

