# Branching

Git branches track different changes seperately
Instead of changing the main project, a branch can be added and then merged once the branch is complete
See what branch you are currently working on with:

    git branch

You can rename a branch with:

    git branch -m oldname newname

You can create a new branch with:

    git branch my_new_brach

### Or

    git switch -c my_new_branch

You use switch to switch branches, the -c flag will create a new branch if it doesn't exist
When a new branch is created, it will use the current commit you are on, so it will also include any commits made before that

## git log --oneline

This command is a great way to see all your branches in a clear concise graph:

    git log --oneline --graph --all

### Example

    * 6fcdcee (HEAD -> main) E: add contents   # main
    | * 8d9156f (add_classics) D: add classics # branch
    |/
    * 26248d3 C: add quotes
    * 4b9caba B: add titles
    * 748228d A: add contents.md




  
