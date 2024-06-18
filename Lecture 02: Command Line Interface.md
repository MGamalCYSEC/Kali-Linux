# Lecture 02: Command Line Interface
## Video Link
[Lecture 01 Video](https://youtu.be/p9CAmV97o7k)

## Command Line (CLI)

The Command Line Interface (CLI) is a text-based interface used for interacting with the Linux operating system. It is a powerful tool for managing the system, performing various tasks, and automating processes. Some of the basic concepts of the CLI include:

### Basic Concepts

- **Commands**: A command is a text-based instruction that tells the system what to do.
- **Options**: Options modify the behavior of a command. They are usually preceded by a hyphen (-) or double hyphen (--).
- **Arguments**: Arguments refer to the inputs provided to a command, which may include files, directories, or any other form of data that the command requires.

### File System Navigation

The Linux file system is organized in a hierarchical structure, with directories (folders) and files. To navigate the file system:

- We can open up a terminal by clicking on the black icon on the top left in the top bar. Once we do so, we get a new window with something similar to the following.

- Switching with the following interface by `ctrl+p`

One commonly used name to refer to the command line or the terminal is a shell. Technically speaking, a shell is a program that processes commands and returns output but it is also used as a synonym for the terminal or console.

### Important Shells on Linux

- **sh**: The Bourne Shell is the foundation for almost all other shell environments since it handles the most important tasks, which have to do with command interpretation or act as a scripting language.
- **Bash**: Also known as Bourne-Again Shell, Bash was developed to serve as a replacement for Bourne Shell by offering additional functionality and better syntax. Bash is the default login shell for most Linux distributions.
- **ksh**: This is another variation of a shell environment called Korn Shell, which again adds some functionality to the basic sh and Bash. For example, ksh handles the loop syntax better than Bash.
### Basic Navigation
``` shell
pwd # will print the current directory (which is helpful if we get lost).
cd  <directory_name> # will take us inside "<directory_name>" within the current folder, if it exists. 
cd.. # This command is used to move up one directory level.
cd / # An absolute path is used to reference a file or directory starting with the root directory (/)
cd ~ # is used to change the current directory to the user's home directory.
file # which checks what type certain file is.
```
``` shell
pwd
/home/kali
file ../../etc/passwd
```

- **zsh**: The Z Shell is an extended Bourne Shell with additional improvements and functionality, which also builds on top of some of the Bash ones.

To determine the currently running shell in a terminal, you can use the following commands:
```bash
echo $0
echo $SHELL
