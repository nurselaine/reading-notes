## Pre-work readings 

#### Linux Tutorial
1. The Command Line: a text-based interface to the system that allows you to enter commands and presents feedback in text
  - enter a command like ls, mkdir etc etc
  - After that, enter command line arguments (<folder name>) 
  - options can come after commands as well, a letter with a dash before is an option: -l -a etc
  - the Shell: this is found within the terminal and defines how the terminal will behave aka how the terminal executes commands (bash is a common shell used - I'm using zsh)
    - use command echo to display which shell is being used
2. Basic Navigation
  - pwd: print working directory command prints the directory that we are currently in 
  - ls: list the contents of the current directory
    - ls can be run with [options] and [location]
    - Options: -l means a long listing will be printed in response which tells us - normal file or d directory, permissions, number of blocks, owner of file/folder, file size, modification time. and actual name of file
  - cd: change directories
    - cd <directory name>: move into specified directory
  - Absolute path: a reference a file/directory in relation to the root directory **begins with a / slash**
  - Relative path: a reference to a file/directory in relation to where we are in the system **does not begin with a slash**
  - linux file structure
    1. root directory : /
    2. subdirectories : <name>/etc...
  - tilde ~ is a shortcut to home directory
  - dot . is a reference to the current directory
  - dot dot .. is a reference to the parent directory
3. More About Files: Everything in linux is a file (even a foler!)
  - Linux = extensionless system : what does that mean?
    - file extension: A set of 2-4 characters at the end of a file name ex (file.exe, file.txt, file.png)
    - Linux ignores this file system and the extension because it looks inside the file and determines what kind of file it is: linux will know how to treat the file even if it is not given an extension name
    - Linux is **case sensitive** while windows is case insensitive
    - Naming files and directories
      - It's ok to add spaces in file names but be cautious because spaces on command lines represent separate items
      - Calling a directory that contains spaces must be called using quotes "<directory/file name>" OR escape characters for the spaces in the name <name>\ <name>
        - tab completion will also resolve spaces in file names
    - hidden files/folders: files that begin with a dot . is hidden
      - unhiding a hidden file: rename file and remove the dot . in the beginning
      - command line option -a: reveals hidden files when using ls -a
4. Manual pages: a set of pages that explain every command available on your system (like an instruction book)
  - man <command to look up> calls the manual page that will respond below the call
  - Keyword searches on manual pages: man -k <search term>
  - long hand and short hand versions of commands: long hand is represented by two dashes -- (--all) while short hand is representated by one dash - (-a). Both options perform the same
5. Making a Directory: mkdir <directory name>
  - the directory name can be a relative or absolute path
  - options 
    - -p: make parent directories as needed
    - -v: makes mkdir tell us what it is doing as it is creating files/folders 
  - deleting files/folders: rmdir [options] <directory name>
    - supports -v and -p options
    - Directory must be empty before it is deleted
  - touch <file name> creates a blank file and may modify the access times on a file (like modifying the last modified time to try and turn in an assignment "on time")
  - cp <file name> <destination name> is to copy a file/folder and move it to a desired place
    - destination: this can be a file or a folder - if it is a file, it will create a copy of the file and name the copy the destination name
    - **to make a cp of a directory use the -r option**
  - Moving a file/folder: mv [option] <source><destination>
      - destination/<new name for source> moving a file into a directory and wanting to give it a new name using mv <source> <destination/new source name>
      - mv can also be used to rename directories/files: mv <source><source/new name>
  - Removing a file: rm [options] <file>
    - options: -r which is 'recursive' which allows us to remove directories and all files and folders contained within the folder: rm -r <folder>

