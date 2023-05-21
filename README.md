A team 0x16. C - Simple Shell project

This is a simple shell written in C using vim. It can execute basic commands and handle signals.

Main functions of a shell:
	Read a line of input from the user using `getline()`.
	Parse the input into tokens using `strtok()`.
	 Execute the tokens as commands using `fork()` and `execvp()`.
	Wait for the child process to finish using `waitpid()`.
	Loop until the user types `exit` or presses `Ctrl-D`.

To create a C - Simple Shell
1.	Create a directory for your project and enter it.
2.	Create a main.c file, Open  with Vim,  write the basic structure of a C program, including the necessary headers and libraries.
3.	Write a loop that will read a line from the standard input using the getline function and store it in a buffer.
4.	Parse the buffer into an array of tokens using the strtok function and a delimiter of your choice (e.g. space or tab).
5.	Take an array of tokens as input and execute them as commands using the fork and execve functions. In addition, handle errors and check for built-in commands (e.g. exit or env).

The fork function creates a new process by duplicating the calling process. The new process is called the child process, and the calling process is called the parent process. The child process inherits most of the attributes of the parent process, but has its own memory space and can execute different code.

The execve function replaces the current process image with a new one specified by a file name, an array of arguments, and an array of environment variables.
6.	 Free the memory allocated by getline and strtok.

This is a useful technique for avoiding memory leaks and improving the performance of your programs.

	getline is a function that reads a line from a file or a stream and stores it in a dynamically allocated buffer.
	strtok is a function that splits a string into tokens based on a delimiter.
	Both functions allocate memory for the buffer and the tokens, and return pointers to them.
	Carefully and Manually free the memory allocated by getline and strtok using a free function to deallocate it.

7.	Test your shell by compiling it with gcc and running it.

Follow the following a few simple steps.
	Write shell code
	Compile the code with gcc
	Run the code with gcc
8.	Add more features to your shell, such as input/output redirection, pipes, aliases, etc..

These features will make your shell more powerful and versatile, and allow you to perform complex tasks with simple commands.

