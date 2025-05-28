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
You can use git log -1 to get the hash of your last commit.

Commit hashes can also be called SHAs because Git uses SHA-1 as a cryptographic hash function

### cat-file Command

Git has a cat-file command that allows you to see the contents of a commit

### Example

    > git cat-file -p 5ba786fcc93e8092831c01e71444b9baa2228a4f

    tree 4e507fdc6d9044ccd8a4a3061324c9f711c4667d
    author ThePrimeagen <the.primeagen@aol.com> 1705891256 -0700
    committer ThePrimeagen <the.primeagen@aol.com> 1705891256 -0700

    A: add contents.md

### Trees and Blobs

- tree: Gits way of storing a directory
- blob: Gits way of storing a file

The contents of the file that was commited will not show when inspecting the commit with cat-file. That is because t is stored in the blob object.

The hash of the blob object can be viewed by running the same git cat-file -p command with the tree hash instead of the commit.

The contents of the blob can be viewed by running the command again with the blob hash.





