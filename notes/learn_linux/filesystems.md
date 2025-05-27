# Filesytems

## What is a Filesystem?

A filesystem organizes data into a hierarchical structure of directories (folders) and files, starting from the root (/). Each user has a home directory. Files store binary data; directories contain files or other directories.

### Examples:

    pwd     # Prints current directory path
    ls      # Lists files/directories in current location
    cd ~    # Moves to user's home directory

## Understanding Filepaths

Filepaths specify the location of files or directories using / to separate levels. Absolute paths start from the root (/), while relative paths start from the current location (. or ..).

### Examples:

    /home/user/docs/report.txt   # absolute path
    ./notes/todo.txt             # relative path
    ../archive                   # one directory up

## Parent Directory
.. refers to the parent directory. Use cd .. to move up one level. From the parent, you can list sibling directories with ls dirname.

### Examples:

    cd ..          # Move up one level  
    ls worldbanc   # List contents of sibling directory

## Absolute vs Relative Paths

- Absolute paths start from the root directory (/) and specify the full location regardless of current directory.
- Relative paths specify a location relative to the current working directory and vary based on where you are.
- Use relative paths for convenience within a known directory context.
- Use absolute paths for clarity when the directory context is unknown or when giving precise file locations.

## Unix Commands
### cat

Displays contents of files sequentially.
Example: cat pets.txt

### head & tail
Show the first or last lines of a file (default 10 lines).
Example: head -n 5 example.txt (first 5 lines)

### less & more
View file content page-by-page interactively; less is more feature-rich.
Example: less -N 2023.csv (view with line numbers)

### touch
Create empty files or update file timestamps.
Example: touch new_document.txt

### mkdir
Create new directories.
Example: mkdir projects

### mv
Move or rename files/directories.
Example: mv old_name.txt new_name.txt

### rm
Delete files or directories (-r for recursive deletion).
Example: rm -r old_projects_directory

### Home Directory (~)
Shortcut to user’s home directory; safe place for personal files.
Example: cd ~

### grep
Search for text within files; supports multiple files and recursive search.
Example: grep "error" server.log

### find
Search files/directories by name or pattern.
Example: find /home/user -name "*.txt"

