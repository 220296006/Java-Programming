# **`Basic Git Commands`**

## 1. **`git init:`**

- **`Purpose:`** Initializes a new Git repository in the current directory.
  - **`Command:`**

     ```bash
     git init
     ```

## 2. **`git clone:`**

- **`Purpose:** Copies a repository from a remote server to the local machine.
  - **`Command:`**

     ```bash
     git clone <repository_url>
     ```

## 3. **`git add:`**

- **`Purpose:** Adds changes in the working directory to the staging area.
  - **`Command:`**

     ```bash
     git add <file_name>
     ```

## 4. **`git commit:`**

- **`Purpose:`** Records changes in the repository and creates a new commit.
  - **`Command:`**

     ```bash
     git commit -m "Commit message"
     ```

## 5. **`git status:`**

- **`Purpose:`** Shows the status of changes as untracked, modified, or staged.
  - **`Command:`**

     ```bash
     git status
     ```

## 6. **`git log:`**

- **`Purpose:`** Displays a log of all commits in the repository.
  - **`Command:`**

     ```bash
     git log
     ```

## 7. **`git branch:`**

- **`Purpose:`** Lists, creates, or deletes branches within a repository.
  - **`Command:`**

     ```bash
     git branch
     ```

## 8. **`git checkout:`**

- **`Purpose:`** Switches between branches or restores working tree files.
  - **`Command:`**

     ```bash
     git checkout <branch_name>
     ```

## 9. **`git merge:`**

- **`Purpose:`** Combines changes from different branches into the current branch.
  - **`Command:`**

     ```bash
     git merge <branch_name>
     ```

## 10. **`git pull:`**

- **`Purpose:`** Fetches changes from a remote repository and merges them into the current branch.
  - **`Command:`**

      ```bash
      git pull origin <branch_name>
      ```

## 11. **`git push:`**

- **`Purpose:`** Updates a remote repository with the changes made locally.
  - **`Command:`**

      ```bash
      git push origin <branch_name>
      ```

## 12. **`git remote:`**

- **`Purpose:`** Manages connections to remote repositories.
  - **`Command:`**

      ```bash
      git remote -v
      ```

## 13. **`git fetch:`**

- **`Purpose:`** Retrieves changes from a remote repository but does not merge them.
  - **`Command:`**

      ```bash
      git fetch origin
      ```

## 14. **`git diff:`**

- **`Purpose:`** Shows changes between commits, commit and working tree, etc.
  - **`Command:`**

      ```bash
      git diff
      ```

These are fundamental Git commands that cover repository initialization, cloning, staging changes, committing, branching, merging, and interacting with remote repositories.

## **`Staging and Commit in Git`**

## 1. **`git add:`**

- **`Purpose:`** Adds changes in the working directory to the staging area.
- **`Command:`**

     ```bash
     git add <file_name>
     ```

## 2. **`git add (all changes):`**

- **`Purpose:`** Adds all changes in the working directory to the staging area.
- **`Command:`**

     ```bash
     git add .
     ```

## 3. **`git add (all changes interactively):`**

- **`Purpose:`** Interactively choose changes to add to the staging area.
- **`Command:`**

     ```bash
     git add -p
     ```

## 4. **`git reset (unstage):`**

- **`Purpose:`** Unstages changes from the staging area, keeping them in the working directory.
- **`Command:`**

     ```bash
     git reset <file_name>
     ```

## 5. **`git commit:`**

- **`Purpose:`** Records changes in the repository and creates a new commit.
- **`Command:`**

     ```bash
     git commit -m "Commit message"
     ```

## 6. **`git commit (with detailed message):`**

- **`Purpose:`** Opens the default text editor to provide a detailed commit message.
- **`Command:`**

    ```bash
     git commit
    ```

## 7. **`git commit (amending):`**

- **`Purpose:`** Adds changes to the previous commit and updates the commit message.
- **`Command:`**

    ```bash
     git commit --amend
    ```

## 8. **`git commit (with specific files):`**

- **`Purpose:`** Commits only the specified files, ignoring changes in others.
- **`Command:`**

    ```bash
     git commit -m "Commit message" <file1> <file2>

    ```

## 9. **`git commit (all changes including untracked):`**

- **`Purpose:`** Commits all changes, including untracked files.
- **`Command:`**

    ```bash
      git commit -a -m "Commit message"

    ```

## 10. **`git commit (adding message in editor):`**

- **`Purpose:`** Opens the default text editor for a detailed commit message.
- **`Command:`**

    ```bash
      git commit
    ```

Staging and committing are essential steps in the Git workflow. Staging allows you to selectively choose changes to include in the next commit, and committing records these changes in the repository with a meaningful message.
