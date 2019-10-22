# Command
## Text Editors
A **text editor** is  piece of software that's downloaded unto the computer. It allows you to write and manage text that's used to build a website.

The most *important features* of a text editor are:
- code completion
- syntax highlighting
- variety of themes
- choosing from a healthy selection of extensions

### Different Text Editors
Every computer comes with its own text editor.
- A **Mac** comes with "Text Edit"
- A **Windows computer** comes with "Notepad"

The original types of text editors don't have the features of code completion, syntax highlighting, themes, or extensions.

Different text editors that you can download are:
- Note Pad ++
- Text Wrangler
- BB Edit
- Visual Studio Code
- Atom
- Brackets
- Sublime Text

### Why Software Developers Use Text Editors
The reason for software developers to use text editors is to essentially make typing the code easier and more decorative. Because with text editors, you can highlight parts of the code for emphasis, the code completion will point out your mistake and fix it for you, and there's different themes and extensions that you can choose from.

## Command Lines
A *command line/terminal* is a test based interface to the system. When commands are entered by being typed on the keyboard, feedback is given to you as text similarly.

### Example:
```
user@bash: ls -l /home/ryan
total 3
drwxr-xr-x 2 ryan users 4096 Mar 23 13:34 bin
drwxr-xr-x 18 ryan users 4096 Feb 17 09:12 Documents
drwxr-xr-x 2 ryan users 4096 May 05 17:25 public_html
user@bash:
```

### Explanation:
- **Line 1:** 
    - After the prompt (user@bash) the command (ls) was entered. A **command** is the first thing you type. Command line arguments are (-l /home/ryan).
    - The command and first command line arguments are separated by a space.
    - The first command line (-l) is referred to as an option. **Options** are used to modify the command's behavior (are listed before other arguments and start with a dash (-)).
- **Line 2-5:**
    - Output for running the command.
- **Line 6:**
    - After the command has been run, the prompt will be displayed for you to enter another command.
        - If the prompt doesn't show, then the command is still running.

### The Shell, Bash
The *Shell* is part of the operating system that determines how the terminal will behave and appear after running commands. 
Bash stands for Bourne again shell.
IF you want to know what shell you're using, use the command (echo).
 - **Echo** displays a system variable that will display your current shell.

#### Example:
```
user@bash: echo $SHELL
/bin/bash
user@bash:
```

## Basic Navigation
- **(pwd)** stands for "Print Working Directory", this displays the directory (folder) you are currently in. 
    - use this command often to know where you are.
- **(ls)** stands for "list", when this command is entered it will display all the folders/directories in the current directory you're located in.
    - when you enter the command (ls /etc) it doesn't just list the current directory, it also lists the directory's contents.
- **(cd)** stands for "change directory". If this command is run without an argument, it'll take you to the home directory.
- **(/etc)** stores config files
- **(/var/log)** stores log files for various system programs
- **(/bin)** the location of several commonly used programs
- **(/usr/bin)** another location for programs on the system

#### Examples:

## Files
