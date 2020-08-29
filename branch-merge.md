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

7. Suppose your remote repository (Github or `origin`) has a branch named `beverages` that you don't have in your local repository.  What is the command to create a new local branch as a copy of the remote `beverages` branch that **tracks** the remote branch?
    There are many commands that do this.  For your own reference you may want to write several.
    ```
    cmd> git fetch
    cmd> git pull
    ```


8. Consider this situation:
   - you have a local repository including a README.md file.
   - Your local repo is up-to-date with a remote Github repo (has identical README.md)
   - You edit README.md on Github using Github's web interface gtand save the changes.
   - On your local machine, you edit README.md, commit the changes and push it to Github.    
   What happens when you push?    
   Explain why.
    ```
    your push was reject.
    this happen because you make change to your remote with counterpart branch and then git request you to update it.
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