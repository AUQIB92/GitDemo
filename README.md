
# Git and GitHub Hands-On Guide

Welcome to the hands-on guide for learning Git and GitHub! This guide will walk you through essential Git commands with examples, so you can get comfortable with version control and collaboration on GitHub.

## Table of Contents

1. [Configuring Git](#configuring-git)
2. [Initializing a Repository](#initializing-a-repository)
3. [Cloning a Repository](#cloning-a-repository)
4. [Checking Repository Status](#checking-repository-status)
5. [Staging Changes](#staging-changes)
6. [Committing Changes](#committing-changes)
7. [Viewing Commit History](#viewing-commit-history)
8. [Branching](#branching)
9. [Switching Branches](#switching-branches)
10. [Merging Branches](#merging-branches)
11. [Deleting a Branch](#deleting-a-branch)
12. [Pushing Changes to Remote](#pushing-changes-to-remote)
13. [Pulling Changes from Remote](#pulling-changes-from-remote)
14. [Fetching Changes](#fetching-changes)
15. [Resetting to a Commit](#resetting-to-a-commit)
16. [Creating a .gitignore File](#creating-a-gitignore-file)
17. [Viewing Differences](#viewing-differences)
18. [Viewing a Specific Commit](#viewing-a-specific-commit)

---

### Configuring Git

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

- **Description**: Sets your name and email for commits. This is a one-time setup for each machine.
- **Example**: After running these commands, any commits you make will use this identity.

---

### Initializing a Repository

```bash
git init
```

- **Description**: Turns an existing directory into a Git repository, creating a hidden `.git` folder.
- **Example**:
   ```bash
   mkdir my-project
   cd my-project
   git init
   ```
- Now, `my-project` is a Git repository.

---

### Cloning a Repository

```bash
git clone [url]
```

- **Description**: Downloads a copy of an existing repository from GitHub or any remote.
- **Example**:
   ```bash
   git clone https://github.com/username/repo-name.git
   ```
- This creates a directory called `repo-name` with all files and commit history.

---

### Checking Repository Status

```bash
git status
```

- **Description**: Shows the status of changes in your working directory (untracked, modified, staged).
- **Example**: Run `git status` to see which files are staged, modified, or untracked.

---

### Staging Changes

```bash
git add [file]
```

- **Description**: Adds changes in a file to the staging area, preparing them for the next commit.
- **Example**:
   ```bash
   echo "Hello, Git!" > hello.txt
   git add hello.txt
   ```

---

### Committing Changes

```bash
git commit -m "Commit message"
```

- **Description**: Records a snapshot of staged changes with a descriptive message.
- **Example**:
   ```bash
   git commit -m "Added hello.txt with greeting message"
   ```

---

### Viewing Commit History

```bash
git log
```

- **Description**: Displays a log of all commits in the current branch.
- **Example**: Run `git log` to see commit messages, authors, and timestamps.

---

### Branching

```bash
git branch [branch-name]
```

- **Description**: Creates a new branch, allowing separate development.
- **Example**:
   ```bash
   git branch feature-branch
   ```

---

### Switching Branches

```bash
git checkout [branch-name]
```

- **Description**: Switches to the specified branch.
- **Example**:
   ```bash
   git checkout feature-branch
   ```

---

### Merging Branches

```bash
git merge [branch-name]
```

- **Description**: Combines the history and changes of one branch into another.
- **Example**:
   ```bash
   git checkout main
   git merge feature-branch
   ```

---

### Deleting a Branch

```bash
git branch -d [branch-name]
```

- **Description**: Deletes the specified branch if it has been merged.
- **Example**:
   ```bash
   git branch -d feature-branch
   ```

---

### Pushing Changes to Remote

```bash
git push
```

- **Description**: Uploads local commits to a remote repository.
- **Example**:
   ```bash
   git push origin main
   ```

---

### Pulling Changes from Remote

```bash
git pull
```

- **Description**: Updates your branch with commits from the remote repository.
- **Example**:
   ```bash
   git pull origin main
   ```

---

### Fetching Changes

```bash
git fetch
```

- **Description**: Downloads commits, files, and refs from a remote repository but doesn’t merge them.
- **Example**:
   ```bash
   git fetch origin
   ```

---

### Resetting to a Commit

```bash
git reset [commit]
```

- **Description**: Moves the current branch to a specified commit, discarding newer commits.
- **Example**:
   ```bash
   git reset --hard abc1234
   ```
- **Caution**: The `--hard` option discards all changes in the working directory.

---

### Creating a .gitignore File

```bash
echo "node_modules/" >> .gitignore
```

- **Description**: Tells Git to ignore specific files or directories, like temporary or dependency files.
- **Example**: Adding `node_modules/` to `.gitignore` prevents that directory from being tracked.

---

### Viewing Differences

```bash
git diff
```

- **Description**: Shows unstaged changes in the working directory.
- **Example**: Run `git diff` to view differences between working directory and staging area.

---

### Viewing a Specific Commit

```bash
git show [commit]
```

- **Description**: Displays the details of a specific commit.
- **Example**:
   ```bash
   git show abc1234
   ```

---

## Additional Resources
For more information, check out these resources:
- [Git Documentation](https://git-scm.com/doc)
- [GitHub Documentation](https://docs.github.com/)
- Pro Git Book: [https://git-scm.com/book/en/v2](https://git-scm.com/book/en/v2)

## Happy Coding!

Share any questions with your instructor or consult the GitHub documentation for additional help.
