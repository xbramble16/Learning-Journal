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

#### Explanation:
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
- **(mv)** stands for "move".
- **(cp)** stands for "copy".
- **(rm)** stands for "remove".
- **(touch)** means to create a new file
- **(mkdir)** stands for "make directory"
- **(file)** obtains information about the type of file for a file/directory.
- **(ls -a)** lists the content of a directory, including the hidden files.
- **(/etc)** stores config files
- **(/var/log)** stores log files for various system programs
- **(/bin)** the location of several commonly used programs
- **(/usr/bin)** another location for programs on the system

#### Examples: 
 - pwd: 
    ```
        user@bash: pwd
        /home/ryan
        user@bash:
    ```
- ls:
    ```
        user@bash: ls
        bin Documents public_html
        user@bash:
    ```
- cd:
    ```
        user@bash: cd (name of directory)
    ```
- mv:
    ```
        user@bash: mv (source) (destination)
    ```
- cp:
    ```
        user@bash: cp (source) (destination)
    ```
- rm:
    ```
        user@bash: rm (name of file)
    ```
- touch:
    ```
        user@bash: (name of file)
    ```
- mkdir: 
    ```
        user@bash: mkdir (name of directory)
    ```
- file:
    ```
        user@bash: file
        Usage: file [-bcEhikLlNnprsvzZ0] [--apple] [--extension] [--mime-encoding] [--mime-type]
        ...
    ```
- ls -a:
    ```
        user@bash: ls -a Documents
        . .. FILE.txt File1.txt file1.TXT .hidden .file.txt
        ...
    ```
- /etc:
    ```
        user@bash: ls /etc
        NetworkManager          init.d                   profile
        X11                     initramfs-tools          profile.d
        acpi                    inputrc                  protocols
        adduser.conf            iproute2                 python
        alternatives            iscsi                    python2.7
        apm                     issue                    python3
        ...
    ```
- /var/log:
    ```
        user@bash: ls /var/log
        alternatives.log  btmp          dpkg.log  landscape  lxd       unattended-upgrades
        apt               dist-upgrade  journal   lastlog    tallylog  wtmp
        ...
    ```
- /bin:
    ```
        user@bash: ls /bin
        bash                false       nc.openbsd     ss
        btrfs               fgconsole   netcat         static-sh
        btrfs-debug-tree    fgrep       netstat        stty
        btrfs-find-root     findmnt     networkctl     su
        btrfs-image         fsck.btrfs  nisdomainname  sync
        ...
    ```
- /usr/bin:
    ```
        user@bash: ls /usr/bin
        2to3-2.7                             newuidmap
        NF                                   ngettext
        VGAuthService                        nice
        '['                                   nl
        aa-enabled                           node
        aa-exec                              nodejs
        ...
    ```

### Paths
A *path* is a way to get a particular file/directory on the system.
Two types of paths are:
- absolute
- relative

The **root directory** is at the very top of the structure. This is denoted by a single slash (/).
- Files could be located in any of these subdirectories.

**Absolute Paths** give a specific location related to the root directory. They can be identified with a forward slash (/).
- Example:
    ```
        user@bash: ls /home/ryan/Documents
        file1.txt file2.txt file3.txt
        ...
    ```

**Relative Paths** give a specific location related to where you are currently in the system. Doesn't begin with a forward slash.
- Example:
    ```
        user@bash: ls Documents
        file1.txt file2.txt file3.txt
        ...
    ```

### More Paths
- (~) *tilde* = shortcut for home directory
- (.) *dot* = reference to current directory
- (..) *dotdot* = reference to parent directory
    - can be used several times to go up to the hierarchy.
        - run **(ls ../../)**
         - would give a listing of root directory
         
## Files
### Linux
*Linux* considers everything (a text file, a directory, keyboard, monitor, etc.) a file.

A **file extension** is commonly known as a set of 2-4 characters after a period at the end of a file.

The following:
- file.exe (program)
- file.txt (plain text file)
- file.png, file.gif, file.jpg (image)
are all common extensions.

Linux is an extensionless system that ignores the extensions and determines the type of file by looking inside. Linux is also case sensitive.

#### Spaces in Names
- **Quotes** = anything inside quotes is considered a single item.
    - Example:
        ```
            user@bash: cd 'Holiday Photos'
            user@bash: pwd
            /home/ryan/Documents/Holiday Photos
        ```
- **Escape Characters** = place a backslash (\) between the two words/characters, doing this escapes/nullifies the special meaning of the next word/character.
    - Example:
        ```
            user@bash: cd Holiday\ Photos
            user@bash: pwd
            /home/ryan/Documents/Holiday Photos
        ```
