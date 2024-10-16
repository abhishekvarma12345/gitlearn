# Amazing Git tutorial
[Check out the Whimsical diagram for high-level overview](https://whimsical.com/embed/KnjyKjhskF2Z1SoQKui6CP@6HYTAunKLgTSyuEcnFk4aAaLzjUSKAcvt4bD6e4YACHqYCg)
## Basic Commands
1. To initialize an empty git repository
    ```bash
    git init
    ```
2. Clone an existing remote repository
    ```bash
    git clone <Your Repo http Url>
    ``` 
3. Setting up the identification info of the code author
   - Check the existing info
    ```bash
    git config --list | grep user.*
    ```
   - Set the indentification parameters(user.name and user.email)
    ```bash
    git config user.name "<Your Name>"
    git config user.name "<Your Email>"
    ```
4. Get the idea about the existing local and remote branches
    ```bash
    git branch -a
    ```
5. Know the tracked/untracked/modified files on a branch
    ```bash
    git status
    ```
6. Adding the files to the staging
   - Add all the changes in the current working directory
    ```bash
    git add .
    ```
   - Add only the changes made in specific files
    ```bash
     git add file1.txt file2.py path/to/file3.txt
    ```
   - Add all the file changes with specific extension
    ```bash
     git add *.ipynb
    ```
7. Commit the staged changes
   ```bash
    git commit -m "<Meaningful message about changes>"
   ```
8. Push the changes to the remote repo
   - pushing for the first time
   ```bash
    git push -u origin <branch name>
   ```
   *Note: The above command set the upstream(-u) repository to the specified remote branch*
  - pushing after setting an upstream repo
    ```bash
    git push
    ```
    *Note: This command can be used once the upstream repo branch is set*

## Advanced Commands
