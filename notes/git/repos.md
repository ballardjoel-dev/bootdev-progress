# Repositories

The very first step of any project is to create a repository, which is essentially a directory that contains a project except it contains one hidden .git directory.
The hidden directory is where Git stores internal tracking and versioning information for the project.
Typically, one repository is made for every new project.

## Creating a new repository

After making a new diretory to store your project run:

    git init

This will create a new repository (repo) and create a hidden .git directory in the project directory, which can be seen with:

    ls -a

## Status command

A file can be in one of three states in a repo.
- untracked (not tracked by Git)
- staged (Marked for inclusion in the next commit)
- committed (Saved to the repo's history)

This command shows the current state of the repo:

    git status

It will tell you which files are untracked, staged or committed

## Staging

Files that are crated need to be staged with:

    git add <path to file | pattern>

This will add the file to the index.

### Example

    git add i-use-arch.btw

## Commit

After staging a file, it can be commited

A commit is a snapshot of the repo at any point and it is how Git keeps track of changes.
A commit comes with a message that describes the changes made in the commit.

### Example

    git commit -m "your message goes here"

If a mistake is made in the message, you can change it with the --amend flag:

    git commit --ammend -m "add contents.md"

## Git log

The git log command shows a history of commits containing:
- Who made a commit
- When the commit was made
- What was changed

### Commit Hash

A commit hash is a string of characters to uniquely identifay each commit
You can refer to any commit hash by using the first seven characters.

Commit hashes can also be called SHAs because Git uses SHA-1 as a cryptographic hash function

