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


