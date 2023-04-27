# Hands-on Lab: Basic Git Commands

## git init

1. Create a new directory for your project
2. Initialize a new Git repository

```bash
$ mkdir git_demo
$ cd git_demo
$ git init
```

## git config

Tell Git who you arex

```
git config --global user.name "YOUR_USERNAME"

git config --global user.email "im_satoshi@musk.com"

git config --global --list
```

## git status

1. Check the status of your repository

```bash
$ git status
```

## git add

1. Create a new file and add some content
2. Add the file to the staging area

```bash
$ echo "Hello, World!" > readme.md
$ git add readme.md
```

## git commit

1. Commit the changes

```bash
$ git commit -m "Initial commit"
```

## git log

1. View the commit history

```bash
$ git log
```

## Uncommit the changes you just did 

- Remove the most recent commit
- Commit again!

```
git reset HEAD~1
```



## git remote

1. Add a remote repository to your local Git repository (use a real repository URL when doing this exercise)

```bash
$ git remote add origin <repository-url>
```

## git push

1. Push your local changes to the remote repository (requires an existing remote repository)

```bash
$ git push -u origin main
```

## git pull

1. Pull changes from the remote repository

```bash
$ git pull origin main
```

## git clone

1. Clone a repository from GitHub (use a real repository URL when doing this exercise)

```bash
$ git clone <repository-url>
```

## git fetch

1. Fetch changes from the remote repository without merging

```bash
$ git fetch origin
```