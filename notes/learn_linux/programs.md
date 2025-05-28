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
