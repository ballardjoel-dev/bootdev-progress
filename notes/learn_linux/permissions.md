# Permissions

## File and Directory Permissions

Permissions control access to files and directories in Unix-like systems.

- Format: -rwxr-xr--
    - First character: - (file) or d (directory)
    - Next 9 characters: grouped as owner/group/others
        - r: read
        - w: write
        - x: execute

- Common patterns:
    - -rwxrwxrwx: Everyone can read, write, and execute.
    - -rwxr-xr-x: Only owner can write; all can read and execute.
    - drwx------: Only owner has full directory access.

## Commands sudo and whoami

### sudo
Executes a command with superuser privileges. Requires proper permissions.

    sudo whoami
    # root

### whoami
Displays the current user’s effective username.

    whoami
    # your_username

## Command chmod
Used to change file or directory permissions ("change mode").

Supports symbolic (u=rwx) or numeric (755) notation.

### Common symbols:
- u: user (owner)
- g: group
- o: others

Add -R to apply changes recursively.

    # Give owner full access, remove all from group/others
    chmod u=rwx,g=,o= mydirectory

## Executable Files
Executable files (like .sh scripts) can be run in Unix-like systems.

Use ./ to run scripts from the current directory.

Use chmod +x to make a file executable, chmod -x to remove that permission.

    chmod +x myscript.sh
    ./myscript.sh
