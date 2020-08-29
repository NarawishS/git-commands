## Part 1. Basics

1. When working with Git locally, what are these?  Describe each one in a sentence
   * Staging area - ```is for files and other transactions waiting to be added/deleted/update in the reposity.```
   * Working copy - ```is a work from local that contains tracked files(files in repo) and untracked files(files from local).```
   * master - ```repository's default branch.```
   * HEAD - ```symbolic reference to the branch you're currently on.```

2. A git commit includes the author's name and email.  How does git know your name and email?  When you install git on a new machine (or in a new user account) you should perform what 2 git commands?
    ```
    # Git configuration commands for a new account
    git config --global user.name "name surname"
    git config --global user.email "user@mail.com"
    ```
3. There are 2 ways to create a local Git repository.  What are they?
    - describe first way (one sentence)
        ```
        cmd> git init 
        to create empty reposity. You must do this inside the project directory.```
    - describe second way
        ```
        cmd> git clone <repo url>
        clone from an existing reposity 
        ```

4. Suppose you create a git repository in a directory (folder) named "/project1". Where does git put the repository files for this project? Write the path to git's files.
    ```
    .../project1/.git/
    ```