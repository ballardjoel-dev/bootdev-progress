# Programs

## Compiled vs Interpreted Languages
Compiled: Source code is translated to machine code before execution.

  - Examples: Go, C, Rust

Interpreted: Source code is executed line-by-line by an interpreter.

  - Examples: Python, Ruby, JavaScript, shell scripts

## Shebang #!
Appears on the first line of a script to specify the interpreter.

  - Format: #! followed by the absolute path to the interpreter.

This is necessary for scripts that need to be interpreted by another program, such as Python or Bash scripts.

    #!/bin/bash     # Bash script
    #!/usr/bin/python3  # Python script

## Bourne Shell (sh)
- sh is the original Unix shell and is POSIX-compliant.
- bash (Bourne Again SHell) adds features to sh and is default on most Linux systems.
- zsh extends sh and is commonly used on macOS.
- All three can run .sh scripts, with bash and zsh offering more interactivity and scripting features.

## Shell Configuration Files
- Shell config files automate shell setup at session start (aliases, variables, etc.).
- Located in ~ and hidden by default (e.g., .bashrc for Bash, .zshrc for Zsh).
- Custom commands added here run automatically when the shell launches.

## Environment Variables in Shell
Environment variables are key-value pairs accessible to the shell and subprocesses.
- Used to pass config info to programs/scripts.
- List variables with env.
- Set variables globally with export VAR=value.
- Access variables with $VAR.
- Temporary variables can be set inline without export for single command scope.

### Examples

    export USER_NAME="Archer"
    echo $USER_NAME
    # Archer
    
### Create a script greet.sh:

    #!/bin/sh
    echo "Hello, $USER_NAME"
    
### Make it executable and run:

    chmod +x ./greet.sh
    ./greet.sh
    # Hello, Archer
    
### Temporarily set a variable for a single command:

    USER_NAME="Lana" ./greet.sh
    # Hello, Lana
    
## Understanding the PATH Variable
PATH is an environment variable listing directories to search for executables.
- Directories are separated by colons :.
- When a command runs, the shell searches these directories in order.
- Without PATH, full executable paths are required (e.g., /bin/ls instead of ls).
- Modifying PATH changes where the shell looks for commands.

### Examples

    echo $PATH
    # /usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin

    export PATH="/usr/local/bin"
    # Temporarily sets PATH to /usr/local/bin only for current session

    source ~/.bash_profile
    # Reloads profile to restore default PATH
