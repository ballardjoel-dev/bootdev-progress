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

You can also use a commit hash to specify where you want to branch off the main line

    git log -c my_new_branch COMMITHASH    

## git log --oneline

This command is a great way to see all your branches in a clear concise graph:

    git log --oneline --graph --all

### Output Example

    * 6fcdcee (HEAD -> main) E: add contents   # main
    | * 8d9156f (add_classics) D: add classics # branch
    |/
    * 26248d3 C: add quotes
    * 4b9caba B: add titles
    * 748228d A: add contents.md

## Merging

        git merge <branch>

This command will merge your branch back onto the main commit line. It does this by finding the merge base commit (the best common ancestor) and replaying the changes from main, starting from the best common ancestor into a new commit, then replaying the changes from the branch onto the main line. It then records the result as a new commit.

# Seeing the merge

The following example is shown after running this command:

    git log --oneline --decorate --graph --parents    

Which returns this:

    *   54dd9b1 6fcdcee 8d9156f (HEAD -> main) F: Merge branch 'add_classics'   # merge
    |\
    | * 8d9156f 26248d3 (add_classics) D: add classics                          # branch
    * | 6fcdcee 26248d3 E: add contents
    |/
    * 26248d3 4b9caba C: add quotes                                             # main
    * 4b9caba 748228d B: add titles
    * 748228d A: add contents.md

(From boot.dev)
Each asterisk * represents a commit in the repository. There are multiple commit hashes on each line because the --parents flag logs the parent hash(es) as well.

- The first line, with these three hashes: 89629a9 d234104 b8dfd64 is our recent merge commit. The first hash, 89629a9 is the merge commit's hash, and the other two are the parent commits.
- The next section is a visual representation of the branch structure. It shows the commits on the add_classics branch and the main branch before the merge. Notice that they both share a common parent.
- The next two lines are just "normal" commits, each pointing to their parent.
- The last line is the initial commit and therefore has no parent.

## Rebase

A rebase is similar to a merge however it actually moves the base of the branch to a new commit on the main.

You must be on the branch to run this:

    git rebase main

This will successfully rebase the branch to the last commit of the main line similar to what is called a fast-forawrd merge.

The benefit of using merge vs using rebase is you can see the full history of the project as in where branches start and then merge back onto main. However over time this canmake the history harder to read. Rebase can make things more linear and easier to understand.

### Warning
You should never rebase a public branch (like main) onto anything else. Other developers have it checked out, and if you change its history, you'll cause a lot of problems for them.

However, with your own branch, you can rebase onto other branches (including a public branch like main) as much as you want.

  
