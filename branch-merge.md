## Part 4. Branch and Merge

1. What is the command to create a new branch named `dev-food`?
    ```
    cmd> git branch dev-food
    ```

2. What is the command to print what your current branch is?
    ```
    cmd> git status
    ```

3. What command to list **all** branches including remote ones?
    ```
    cmd> git branch -a
    ```

4. What is command to switch your working copy to a branch named `dev-food`?
    ```
    cmd> git checkout dev-food
    ```

5. You commit some files to `dev-food` and try to "push" them to Github, but it fails:

    ```
    cmd>  git checkout dev-food
    cmd>  git push
    fatal:  The current branch dev-food has no upstream branch. 
    ```
    Explain this error.
    ```
    The current branch didn't set the remote as upstream.
    ```

6. What is the command to push `dev-food` to `origin` as a new remote branch on `origin`?
    ```
    cmd> git push --set-upstream origin dev-food
    ```

## Viewing Changes and Commits

* Command to show the history of a repository in the terminal (command) window.  This form shows one line per commit, with a graph, and all branches.
    ```
    git log --oneline --graph --all
    ```
    Some versions of git have an *alias* "log1" for this (`git log1`).

* The GUI tool `gitk` or `gitk --all` displays even more info about the commit history.


* The output of `git diff` can be hard to read. To view differences more visually:

    1. View differences on Github.
    2. Meld or Diffuse to compare and merge files. `git difftool` lists more tools.
    3. `gitk` shows diffs between commits
    4. Eclipse EGit shows side-by-side diffs and can merge interactively