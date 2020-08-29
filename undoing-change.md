## Part 3. Undoing Changes

1. Use an editor to make some changes to file `a`.  What is the command to view the **differences** between your working copy `a` and the current version in repository?
    ```
    cmd> git diff HEAD a

    cmd> git diff HEAD <sorce>
    ```

2. You decide you don't like the changes to `a`. What is the command to **replace** your working copy of `a` with the current version in the repository?    
    (This also works if you accidentally *delete* a file from your working copy.)
    ```
    cmd> git restore a
    ```

3. How do you "undo" a commit?  What is the command to move the "head" of the current branch to the **previous** commit?
    ```
    cmd> git checkout HEAD~1
    ```