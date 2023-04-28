# Git Lab Session: Rebasining, Branching, Pull Requests, and Merging with GitHub

## Introduction

In this lab session, you will learn about advanced rebasing

## Prerequisites

Before you begin this lab session, you should have:

- A basic understanding of Git and GitHub
- A GitHub account
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

### Step 2: Create a new branch

1. Enter the following command to create a new branch:

```bash
git checkout -b feature/advanced-rebase
```

2. Make some changes to the code and commit the changes:

```bash
git add .
git commit -m "Add new feature"
```

3. Make some more changes to the code and commit the changes:

```bash
git add .
git commit -m "Add another feature"
```

4. Make some more changes to the code and commit the changes:

```bash
git add .
git commit -m "Add yet another feature"
```

5. Check the log to see the commit history:

```bash
git log --oneline
```

### Step 3: Switch to the master branch

1. Enter the following command to switch to the master branch:

```bash
git checkout master
```

2. Make some changes to the code and commit the changes:

```bash
git add .
git commit -m "Update master branch"
```

### Exercise: Advanced Rebasing Scenarios

In this exercise, you will learn about more advanced rebasing scenarios, including reordering, squashing, and rewriting commits. Follow the steps below to complete the exercise:

1. Switch back to the `feature/advanced-rebase` branch:

```bash
git checkout feature/advanced-rebase
```

2. Enter the following command to reorder the last two commits:

```bash
git rebase -i HEAD~2
```

3. In the interactive rebase editor, change the order of the two commits and save the file.

4. Enter the following command to squash the last two commits into one:

```bash
git rebase -i HEAD~2
```

5. In the interactive rebase editor, replace the word "pick" with "squash" for the second commit and save the file.

6. Enter the following command to rewrite the commit message:

```bash
git commit --amend -m "Add new and improved feature"
```

7. Check the log to see the updated commit history:

```bash
git log --graph --oneline
```

8. Enter the following command to force push the changes to the remote repository:

```bash
git push -f origin feature/advanced-rebase
```

9. Create a pull request to merge the `feature/advanced-rebase` branch



## Activity

consider you made 5 commits to a file, Will need you to try and squash 2 of those commits and rewrite the commit message on one of them in a interactive rebase