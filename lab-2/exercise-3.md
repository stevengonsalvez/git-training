# Git Lab Session: Merge Conflicts

## Introduction

In this lab session, you will learn how to handle merge conflicts in Git. You will use the Git command line interface (CLI) to complete the lab.

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

### Step 2: Create a new branch and make changes

1. Enter the following command to create a new branch and switch to it:

```bash
git checkout -b feature/merge-conflict
```

2. Make some changes to the code and commit the changes:

```bash
git add .
git commit -m "Add new feature"
```

### Step 3: Switch to the master branch and make changes

1. Enter the following command to switch to the master branch:

```bash
git checkout master
```

2. Make some changes to the same code file and commit the changes:

```bash
git add .
git commit -m "Update master branch"
```

### Step 4: Merge the changes and resolve conflicts

1. Enter the following command to merge the changes from the `feature/merge-conflict` branch:

```bash
git merge feature/merge-conflict
```

2. You will receive a message saying that there are merge conflicts. Enter the following command to open the file with the conflicts:

```bash
git status
```

3. Open the file with the conflicts in your text editor and resolve the conflicts by editing the file to remove the conflict markers and selecting which version of the code to keep.

4. Enter the following commands to stage and commit the resolved conflicts:

```bash
git add <filename>
git commit -m "Resolve merge conflict"
```

### Conclusion

Congratulations! You have successfully resolved a merge conflict in Git.