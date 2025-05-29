# Git Config

Git stores author information when making a commit so it shows who made changes to the repo.

Below is an example on how to update the global configuration:

    git config --add --global user.name "ThePrimeagen"
    git config --add --global user.email "the.primeagen@aol.com"

Taking the command apart:

- git config: The command to interact with your Git configuration.
- --add: Flag stating you want to add a configuration.
- --global: Flag stating you want this configuration to be stored globally in your ~/.gitconfig. The opposite is "local", which stores the configuration in the current repository only.
- user: The section.
- name: The key within the section.
- "ThePrimeagen": The value you want to set for the key.

Any old data can be stored in the git config, but git only actually uses specific keys

    git config --list --local

This command lists the local config

    git config --get <key>

This command gets one specific key in the format <section.keyname>.

The --unset flag removes a config value:

    git config --unset <key>

There are several locations where Git can be configured. From more general to more specific, they are:

- system: /etc/gitconfig, a file that configures Git for all users on the system
- global: ~/.gitconfig, a file that configures Git for all projects of a user
- local: .git/config, a file that configures Git for a specific project
- worktree: .git/config.worktree, a file that configures Git for part of a project

For reference, global overrides system, local overrides global, and worktree overrides local.

