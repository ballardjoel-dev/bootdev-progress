# Terminals and Shells

## Terminals vs. GUI (CLI vs. GUI)
A CLI (Command Line Interface) lets users interact with the system using text commands, offering speed, automation, and precision—especially for repetitive or complex tasks. A GUI (Graphical User Interface) uses visual elements like windows and icons, which are more beginner-friendly but less efficient for scripting and automation.

### Example:

    echo "Hello world"
    # Outputs: Hello world

## What is a Shell

A shell is a command-line program that reads, evaluates, and executes user input—often described as a REPL (Read-Eval-Print Loop). It serves as a bridge between the user and the operating system, letting you run commands, manage files, and control system processes.

### Examples of Shells:

- bash (common on Linux)
- zsh (popular alternative to bash)
- PowerShell (primarily used on Windows)

## Variables in Shell Scripts

Shell variables store values like strings, numbers, or paths using the syntax name=value (no spaces). Access them with $name. Shell variables are untyped and useful for reuse within scripts.

### Example:

    company="WorldBanc"
    year_founded="1969"
    ceo_name="Jeff Gates"

    echo "$company was founded in $year_founded by $ceo_name"
    # Output: WorldBanc was founded in 1969 by Jeff Gates

## Shell Command History

The history command shows previously run commands in the terminal session. Use ↑/↓ arrow keys to navigate command history. Use clear or Ctrl + L to clear the screen without deleting history.

### Example:

    history      # Shows command history
    clear        # Clears terminal screen

