# Git Lab Session: Ignoring Files with .gitignore

## Introduction

In this lab session, you will learn how to use the .gitignore file to ignore files in Git. You will use the Git command line interface (CLI) to complete the lab.

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

### Step 2: Create a new file and commit it

1. Enter the following command to create a new file:

```bash
touch <filename>
```

2. Add some content to the file and save it.

3. Enter the following commands to add and commit the file:

```bash
git add <filename>
git commit -m "Add new file"
```

### Step 3: Create a .gitignore file

1. Enter the following command to create a new file called .gitignore:

```bash
touch .gitignore
```

2. Open the .gitignore file in your text editor and add the following line:

```bash
<filename>
```

3. Save and close the file.

### Step 4: Add and commit the .gitignore file

1. Enter the following commands to add and commit the .gitignore file:

```bash
git add .gitignore
git commit -m "Add .gitignore file"
```

### Step 5: Verify that the file is ignored

1. Enter the following command to make a change to the file:

```bash
echo "Some changes" >> <filename>
```

2. Enter the following command to check the status of the repository:

```bash
git status
```

3. You should see that the changes to the file are not being tracked.

### Conclusion

Congratulations! You have successfully learned how to use the .gitignore file to ignore files in Git.