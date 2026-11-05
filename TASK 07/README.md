Aim:
To study process creation and management in an operating system using fork(), exec(), waitpid() and _exit() system calls.

Alternative Concept:
An alternative to using fork() followed by exec() is posix_spawn(). It creates a new process and executes a program in a single operation.

Method	Description
fork() + exec()	Creates a child process and then executes another program.
posix_spawn()	Creates a process and executes a program in one operation.
Comparison:
•	fork() + exec() provides separate control over process creation and program execution.
•	posix_spawn() provides a simpler way to create and execute a process.
•	Both methods can be used to execute external programs.
Conclusion:
Thus, process creation and management were studied successfully using fork(), exec(), waitpid() and _exit(). The program demonstrates how a parent process creates child processes, executes programs and collects their exit statuses.


