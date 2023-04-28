# Git Lab Session: Git Aliases

## Introduction

In this lab session, you will learn how to use Git aliases to create shortcuts for common Git commands. You will use the Git command line interface (CLI) to complete the lab.

## Prerequisites

Before you begin this lab session, you should have:

- A basic understanding of Git
- Git installed on your local machine

## Lab Session

### Step 1a: Fork the repository

1. Go to the example repository: https://github.com/stevengonsalvez/git-training
2. Click the "Fork" button in the top-right corner of the page.
3. Select your GitHub account as the destination for the fork.

### Step 1b: Clone the forked repository

1. In your forked repository, click the green "Code" button and copy the HTTPS URL.
2. Open a terminal or Git Bash and navigate to the directory where you want to clone the repository.
3. Enter the following command to clone the repository:

```bash
git clone <HTTPS URL>
```

### Step 2: Create a Git alias

1. Enter the following command to create a Git alias for the `log` command:

```bash
git config --global alias.l "log --oneline --decorate --graph"
```

### Step 3: Test the Git alias

1. Enter the following command to test the Git alias:

```bash
git l
```

2. You should see a list of the commit history in a more readable format.

### Step 4: Create a more complex Git alias

1. Enter the following command to create a more complex Git alias that adds, commits, and pushes changes in one command:

```bash
git config --global alias.acp "!git add -A && git commit -m && git push"
```

### Step 5: Test the more complex Git alias

1. Enter the following command to test the more complex Git alias:

```bash
git acp "Add and commit changes"
```

2. You should see the changes added, committed, and pushed to the remote repository.

### Conclusion

Congratulations! You have successfully learned how to use Git aliases to create shortcuts for common Git commands.


## Activity

Try defining aliases for additional commands merge, rebase , branch etc.