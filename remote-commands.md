## Part 5. Commands for Remotes
1. The command to list all your remote repositories, with their URL.

2. The command to view details about a rempote repo named origin, including all the remote banches, and local tracking branches.

3. Suppose your remote repository (Github or `origin`) has a branch named `beverages` that you don't have in your local repository.  What is the command to create a new local branch as a copy of the remote `beverages` branch that **tracks** the remote branch?
    There are many commands that do this.  For your own reference you may want to write several.
    ```
    cmd> git fetch
    cmd> git pull
    ```

4. Consider this situation:
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

5. What are the steps to resolve the problem in the previous problem?

6. Suppose you want to move origin to a different URL. This can happen if you change the name of a repo on Github, or transfer ownership from one person to another. What is the command to change the URL for origin to https://github.com/your_name/newrepo.