# Git Lab Session: Rebasing, Branching, Pull Requests, and Merging with GitHub

## Introduction

In this lab session, you will learn about some advanced Git features, including rebasing, branching, pull requests, and merging with GitHub. You will use the Git command line interface (CLI) and GitHub web interface to complete the lab.

## Prerequisites

Before you begin this lab session, you should have:

- A basic understanding of Git and GitHub
- A GitHub account
- Git installed on your local machine

## Lab Session

### Step 1: Fork the repository

1. Go to the example repository: https://github.com/stevengonsalvez/git-training
2. Click the "Fork" button in the top-right corner of the page.
3. Select your GitHub account as the destination for the fork.

### Step 2: Clone the forked repository

1. In your forked repository, click the green "Code" button and copy the HTTPS URL.
2. Open a terminal or Git Bash and navigate to the directory where you want to clone the repository.
3. Enter the following command to clone the repository:

```bash
git clone <HTTPS URL>
```

### Step 3: Create a new branch

1. Navigate to the cloned repository directory.
2. Enter the following command to create a new branch:

```bash
git checkout -b feature/new-branch
```

### Step 4: Make changes to the code

1. Open the code files in a text editor.
2. Make some changes to the code, such as adding a new function or fixing a bug.
3. Save the changes.

### Step 5: Commit the changes

1. Enter the following command to stage the changes:

```bash
git add .
```

2. Enter the following command to commit the changes:

```bash
git commit -m "Add new feature"
```

### Step 6: Make a change in the master branch

1. Enter the following command to switch to the master branch:

```bash
git checkout master
```

2. Open the code files in a text editor.
3. Make some changes to the code, such as adding a new function or fixing a bug.
4. Save the changes.

5. Enter the following commands to stage and commit the changes:

```bash
git add .
git commit -m "Update master branch"
```

### Step 7: Rebase the branch

1. Enter the following command to update the master branch:

```bash
git fetch origin master
```

2. Enter the following command to rebase the feature branch:

```bash
git rebase origin/master feature/new-branch
```

### Step 8: Push the changes to GitHub

1. Enter the following command to push the changes to your forked repository:

```bash
git push origin feature/new-branch
```

### Step 9: Create a pull request

1. Go to the forked repository on GitHub.
2. Click the "New pull request" button.
3. Select the base repository and branch you want to merge your changes into.
4. Review the changes and add a description of the changes.
5. Click the "Create pull request" button.

### Step 10: Merge the pull request

1. Once the pull request has been reviewed and approved, click the "Merge pull request" button.
2. If there are any conflicts, resolve them and then click the "Confirm merge" button.

### Step 11: Update the local repository

1. Enter the following command to update your local repository:

```bash
git pull origin master
```


## Activity

Instead of `git rebase origin/master feature/new-branch` execute `git merge origin/master feature/new-branch` and observe the difference
Try to summarize the difference between a `merge` and a `rebase`