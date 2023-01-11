# Git Cheat Sheet

## Git Configuration

- ``` git config --global user.name "Your Name" ``` : Set your name for all Git repositories on your computer
- ``` git config --global user.email "your@email.com" ``` : Set your email for all Git repositories on your computer

## Creating and Cloning Repositories

- ``` git init ``` : Initialize a new Git repository in the current directory
- ``` git clone <url> ``` : Clone a remote repository and create a local copy on your computer

## Making Changes

- ``` git status ``` : View the status of your repository, including modified and untracked files
- ``` git add <filename> ``` : Stage a file for commit
- ``` git add . ``` : Stage all modified and untracked files for commit
- ``` git commit -m "commit message" ``` : Commit your staged changes with a message
- ```git diff ``` : View differences between your staged changes and the last commit

## Viewing History

- ``` git log ``` : View the commit history for the current branch
- ```git log --oneline ``` : View the commit history in a condensed format
- ```git show <commit> ``` : View the changes made in a specific commit

## Branching and Merging

- ``` git branch ``` : View a list of all branches in the repository
- ``` git branch <branch> ``` : Create a new branch
- ``` git checkout <branch> ``` : Switch to a different branch
- ``` git merge <branch> ``` : Merge a branch into the current branch
- ``` git branch -d <branch> ``` : Delete a branch

## Remote Repositories

- ``` git push ``` : Push your local commits to the remote repository
- ``` git pull ``` : Pull the latest commits from the remote repository
- ``` git fetch ``` : Download the latest commits from the remote repository, but don't integrate them into your local branch

## Resolving Conflicts

If you try to merge two branches and Git detects a conflict, you'll need to resolve the conflict manually. Here are some steps to follow:

1. Open the conflicting file and look for the conflict markers ``` <<<<<<< ``` , ``` ======= ``` , and ``` >>>>>>> ``` . The text between ``` <<<<<<< ``` and ``` ======= ``` is the version from your current branch, and the text between ``` ======= ``` and ``` >>>>>>> ``` is the version from the branch you're trying to merge.
2. Edit the file to resolve the conflict by deciding which changes to keep and deleting the conflict markers.
3. Stage the file for commit using ``` git add <filename> ``` .
4. Commit the file using ``` git commit -m "Resolve conflict" ``` .

## Undoing Changes

- ```git revert <commit> ``` : Undo the changes made in a specific commit, creating a new commit to record the reversal
- ``` git reset <commit> ``` : Undo commits by moving the branch pointer to a previous commit and discarding commits in the process. Be careful with this, as the discarded commits are permanently lost.

## Commands the author use most of the time: 

1. Clone a repository:

``` git clone <repository url> ```

2. Check the status of your repository:

``` git status ```

3. Add files to the staging area:

``` git add <file1> <file2> ... ```

Or Add all files to the staging area:

``` git add . ```

4. Commit changes with a message:

``` git commit -m "commit message" ```

5. Push changes to a remote repository:

``` git push ```

6. Pull the latest changes from a remote repository:

``` git pull ```

7. Create a new branch:

``` git branch <branch name> ```

8. Switch to a different branch:

``` git checkout <branch name> ```

9. Merge one branch into another:

``` git merge <branch name> ```

10. Undo local changes:

``` git stash ```

11. Discard commits and move the branch pointer to a previous commit:

``` git reset --hard HEAD~<number of commits> ```

12. Initialize a new Git repository:

``` git init ```

13. View commit history:

``` git log ```

## For a complete list and most detailed information, you can refer to the Git documentation or use this command:

``` git --help```

## Resources

- [Git Official Docs](https://git-scm.com/docs)
- [7 tips for improving your productivity with Git](https://dev.to/dgenezini/7-tips-for-improving-your-productivity-with-git-ajg)

## Screenshots

<img width="800" alt="Screenshot 2022-12-29 at 10 31 20 PM" src="https://user-images.githubusercontent.com/89284873/210034676-eb993e9d-11fc-46a8-b4ff-263f483f9cfa.png">

<img width="800" alt="Screenshot 2022-12-29 at 10 31 39 PM" src="https://user-images.githubusercontent.com/89284873/210034693-1603e926-4996-4588-8934-635a7f2d48c7.png">
