# **`Inspecting and Undoing Changes in Git`**

**1. `git status`:**

- **`Purpose:`** Shows the status of changes as untracked, modified, or staged.
- **`Command:`**

     ```bash
     git status
     ```

**2. `git diff`:**

- **`Purpose:`** Shows changes between the working directory and the staging area.
- **`Command:`**

     ```bash
     git diff
     ```

**3. `git diff (specific file)`:**

- **`Purpose:`** Shows changes for a specific file between the working directory and the staging area.
- **`Command:`**

     ```bash
     git diff <file_name>
     ```

**4. `git diff (between commits)`:**

- **`Purpose:`** Shows changes between two commits.
- **`Command:`**

     ```bash
     git diff <commit_hash1> <commit_hash2>
     ```

**5. `git log`:**

- **`Purpose:`** Displays a log of all commits in the repository.
- **`Command:`**

     ```bash
     git log
     ```

**6. `git log (specific file)`:**

- **`Purpose:`** Displays commit history for a specific file.
- **`Command:`**

```bash
 git log -- <file_name>
```

**7. `git reset (unstage)`:**

- **`Purpose:`** Unstages changes from the staging area, keeping them in the working directory.
- **`Command:`**

     ```bash
     git reset <file_name>
     ```

**8. `git checkout (discard changes in working directory)`:**

- **`Purpose:`** Discards changes in the working directory for a specific file.
- **`Command:`**

```bash
git checkout -- <file_name>
```

**9. `git reset (discard changes in staging area)`:**
    - **`Purpose:`** Discards changes in the staging area.
    - **`Command:`**

```bash
      git reset
```

**10. `git revert`:**
    - **`Purpose:`** Creates a new commit that undoes the changes made in a previous commit.
    - **`Command:`**

```bash
      git revert <commit_hash>

```

**11. `git reset (hard reset to a specific commit)`:**
    - **`Purpose:`** Resets the branch and working directory to a specific commit, discarding all changes.
    - **`Command:`**

```bash
      git reset --hard <commit_hash>
```

**12. `git clean`:**
    - **`Purpose:`** Removes untracked files from the working directory.
**`Purpose:`**

```bash
      git clean -fd

```

Inspecting changes using `git diff` and undoing changes using various commands like `git reset`, `git checkout`, and `git revert` are essential for managing the state of a Git repository and ensuring code quality.

## **Collaborating in Git**

**1. `git clone`:**

- **`Purpose:`** Copies a repository from a remote server to the local machine.
- **`Command:`**

     ```bash
     git clone <repository_url>
     ```

**2. `git remote`:**

- **`Purpose:`** Manages connections to remote repositories.
- **`Command:`**

     ```bash
     git remote -v
     ```

**3. `git fetch`:**

- **`Purpose:`** Retrieves changes from a remote repository but does not merge them.
- **`Command:`**

     ```bash
     git fetch origin
     ```

**4. `git pull`:**

- **`Purpose:`** Fetches changes from a remote repository and merges them into the current branch.
- **`Command:`**

     ```bash
     git pull origin <branch_name>
     ```

**5. `git push`:**

- **`Purpose:`** Updates a remote repository with the changes made locally.
- **`Command:`**

     ```bash
     git push origin <branch_name>
     ```

**6. `git branch`:**

- **`Purpose:`** Lists, creates, or deletes branches within a repository.
- **`Command:`**

     ```bash
     git branch
     ```

**7. `git merge`:**

- **`Purpose:`** Combines changes from different branches into the current branch.
- **`Command:`**

     ```bash
     git merge <branch_name>
     ```

**8. `git checkout`:**

- **`Purpose:`** Switches between branches or restores working tree files.
- **`Command:`**

     ```bash
     git checkout <branch_name>
     ```

**9. Pull Request (PR):**

- **`Purpose:`** A way to propose changes from one branch to another. It allows for review and discussion before merging.
- **`Command:`** (Typically done on platforms like GitHub or GitLab)
  - Open a new pull request.
  - Request reviews and collaborate with team members.

Collaborating in Git involves cloning repositories, managing remotes, fetching and pulling changes, pushing changes to remotes, branching, merging, and utilizing pull requests for code review and integration.

## **`Collaborating in Git`**

**1. `git clone`:**

- **`Purpose:`** Copies a repository from a remote server to the local machine.
- **`Command:`**

     ```bash
     git clone <repository_url>
     ```

**2. `git remote`:**

- **`Purpose:`** Manages connections to remote repositories.
- **`Command:`**

     ```bash
     git remote -v
     ```

**3. `git fetch`:**

- **`Purpose:`** Retrieves changes from a remote repository but does not merge them.
- **`Command:`**

     ```bash
     git fetch origin
     ```

**4. `git pull`:**

- **`Purpose:`** Fetches changes from a remote repository and merges them into the current branch.
- **`Command:`**

     ```bash
     git pull origin <branch_name>
     ```

**5. `git push`:**

- **`Purpose:`** Updates a remote repository with the changes made locally.
- **`Command:`**

     ```bash
     git push origin <branch_name>
     ```

**6. `git branch`:**

- **`Purpose:`** Lists, creates, or deletes branches within a repository.
- **`Command:`**

     ```bash
     git branch
     ```

**7. `git merge`:**

- **`Purpose:`** Combines changes from different branches into the current branch.
- **`Command:`**

     ```bash
     git merge <branch_name>
     ```

**8. `git checkout`:**

- **`Purpose:`** Switches between branches or restores working tree files.
- **`Command:`**

     ```bash
     git checkout <branch_name>
     ```

**9. `Pull Request (PR):`**

- **`Purpose:`** A way to propose changes from one branch to another. It allows for review and discussion before merging.
- **`Command:`**
(Typically done on platforms like GitHub or GitLab)
  - Open a new pull request.
  - Request reviews and collaborate with team members.

Collaborating in Git involves cloning repositories, managing remotes, fetching and pulling changes, pushing changes to remotes, branching, merging, and utilizing pull requests for code review and integration.
