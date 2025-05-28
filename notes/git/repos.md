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

