# Whats happening

<!-- slide bg="https://images.unsplash.com/photo-1633976976526-4e3584e91a5d?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2340&q=80" -->

<!-- .slide: style="color: white;" -->
<!-- slide style="font-size: 30px" -->
- Git 
	- How git works
	- fundamental elements
	- basic commands
	- hands on with git 
- Github
	- hands on with remote code on github
	- github components
		- actions, security
		- codespace, copilot
		- issues and project management

--

### Why Git in Engineering

![[../../Attachments/Pasted image 20230427194758.png]]

note: my notes

- Everything is about creation of code, to the speed which that code can be realised and made reachable with the best experience to the users


--

### Engineering cont.


<!-- element align="left" -->From Ideation
</br>

1. Everything as code

1. Continuous Everything
2. Continuous observability

You would hear the word *GITOPS* which encapsulates the last three

note: 
- documentation, architecture, infrastructure, code , tests, security for scanning the code
- continuous is how many touches before anything that is coded is available to the user
- continuous observation and ensuring the solution is reachable for the user

---
<!-- slide bg="purple" -->
<!-- slide style="font-size: 30px" -->
## So what is Git

- Version control

- distributed : every user “clones” a copy of a repository (a collection of files) and has the **_full_** history of the project on their own hard drive
- synchronise code between multiple people

note: 
- it is basically the history tab of the code editor
- If at any point while coding you hit a fatal error and don’t know what’s causing it you can always revert back to the stable state
- you and your friend are collaborating on a project. You both are working on the same project files. Now Git takes those changes you and your friend made independently and merges them to a single “**Master**” repository. So by using Git you can ensure you both are working on the most recent version of the repository.


--

<!-- slide style="font-size: 30px" -->
### Fundamental Components of GIT

- Repository : Collection of code

- Branches: Branches allow you to work on different versions of your code simultaneously. They are like separate timelines where you can make changes without affecting the main branch.
- Tags: A tag is a way to mark a specific commit as important. It is often used to mark a release or a major milestone in your project
- Remote: A remote is a connection to a repository hosted on a remote server. You can push and pull changes to and from a remote repository.
- workflow: refers to the process and methodology that a team or individual uses to manage changes to a codebase
- commit: commit is a snapshot of the changes made to a file or set of files. Each commit has a unique identifier and a commit message that describes the changes made. A commit is immutable.

note: 
1.  Centralized Workflow: This workflow is based on a central repository where all changes are made and reviewed before being merged into the main branch.
    
2.  Feature Branch Workflow: This workflow involves creating a new branch for each feature or issue being worked on. Developers work on their respective branches and merge them back into the main branch when ready.
    
3.  Gitflow Workflow: This workflow is similar to the Feature Branch Workflow but introduces two additional branches for release management. It has a more complex branching strategy that allows for parallel development, hotfixes, and long-term maintenance.
    
4.  Forking Workflow: This workflow involves creating a personal copy (fork) of a repository and making changes independently. When ready, changes are submitted to the original repository as pull requests.
    
5.  Pull Request Workflow: This workflow is based on the use of pull requests to submit changes for review and merging. It is commonly used in open source projects where many contributors are involved.

--

### Simple Git Workflow

![[../../Attachments/Pasted image 20230427205014.png]]

note:
**If you consider a file in your Working Directory, it can be in three possible states.**

1.  **It can be staged.** Which means the files with the updated changes are marked to be committed to the local repository but not yet committed.
2.  **It can be modified**. Which means the files with the updated changes are not yet stored in the local repository.
3.  **It can be committed**. Which means that the changes you made to your file are safely stored in the local repository.

--

<!-- slide style="font-size: 25px" -->
### Git basic commands

-   `git add` is a command used to add a file that is in the working directory to the staging area.

-   `git commit` is a command used to add all files that are staged to the local repository.
-   `git push` is a command used to add all committed files in the local repository to the remote repository. So in the remote repository, all files and changes will be visible to anyone with access to the remote repository.
-   `git fetch` is a command used to get files from the remote repository to the local repository but not into the working directory.
-   `git merge` is a command used to get the files from the local repository into the working directory.
-   `git pull` is command used to get files from the remote repository directly into the working directory. It is equivalent to a `git fetch` and a `git merge` .

---
<!-- slide bg="#157394" -->
<!-- slide style="font-size: 30px" -->

## What is Github

- To get started with some labs, will start with 
  
	- github being a remote repository hosting solution that allows many users to easily collaborate through the internet.


> ps: Github is not the only remote provider , there are plenty of other similar remote git hosted solutions - gitlab, bitbucket, azure repos, aws code commit<!-- element style="background:grey" -->

> Also git is not the only version control system. Git is the most popular and most used. Other's used are <!-- element style="background:grey" -->
> - subversion based <!-- element style="background:grey" -->
> - mercurial<!-- element style="background:grey" -->
> - perforce<!-- element style="background:grey" -->

--
<!-- slide style="font-size: 20px" -->
### What else is github

-  Version control: 
    
-  Collaboration: GitHub allows developers to collaborate on code by contributing to each other's repositories, discussing issues, and reviewing code changes through pull requests.
- Development: 
	- Codespaces
	- Copilot
	    
-  Project management: GitHub offers tools for managing projects, including task tracking, issue management, and project boards.
    
-  Continuous integration and deployment: 
	- Github Actions
	- Also integrations with webhooks and events, OIDC federation into other continuous integration tools

- Code Security
	- dependabot
	- github advanced security
		    
- Community: GitHub has a large community of developers who share code, contribute to open source projects, and offer support and guidance to others.

---
<!-- slide bg="https://picsum.photos/seed/picsum/800/600" data-background-opacity="0.5" -->
##  Lab - 1

- Go through some basic workflows without GUI
- operate on a local repository
- operate on a remote repository

</br>

### Prerequisites

- git installed
- Go to this [**link**](https://www.apple.com/macos/what-is/) or this **[link](https://gitforwindows.org/)** for more info on how to get it
- github account and setup [here](https://github.com/stevengonsalvez/git-training/blob/main/lab-1/pre-req.md)

--
<!-- slide bg="#157394" -->
### What you learned Lab-1

- adding and committing to local repository
- undoing a commit
- pushing to a remote
- cloning a remote repository to your workspace

---
<!-- slide bg="https://images.unsplash.com/photo-1630959305606-3123a081dada?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=987&q=80" data-background-opacity="0.3" -->
## Lab-2

- Collaborating
	- branching
	- pull requests
	- merging, merge conflicts
	- stashing, rebasing
- gitignore
- branching and gitflow

--
<!-- slide bg="#157394" -->
### What you learned Lab-2


- How to collaborate across the team
- How to fix mistakes across the histor

---
<!-- slide bg="https://images.unsplash.com/photo-1518842013791-b874be246c34?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=988&q=80" data-background-opacity="0.3" -->

<!-- slide style="font-size: 30px" -->
## Lab-3

Advanced git: fixing complex commit mistakes in the history

-   git bisect
-   git cherry-pick
-   git reset
-   git reflog
-   merge strategies
    -   fast forward
    -   recursive
    -   octopus
-   identity and commit verification
-   hooks (pre and post)

--
<!-- slide bg="#157394" -->
### What you learned Lab-3

- search complex code to find in history of the code
- complex merge conflicts and advanced selective merging
- reverting local messes and lost commits

---

<!-- slide bg="https://images.unsplash.com/photo-1576086213369-97a306d36557?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8MzJ8fGxhYnxlbnwwfHwwfHw%3D&auto=format&fit=crop&w=800&q=60" data-background-opacity="0.3" -->
<!-- slide style="font-size: 30px" -->
## Lab-4

Github setup

-   git flow : for continuous delivery, continuous deploy, release trains
    -   example: trunk based workflow, feature branch workflow
- Github settings:
	- branch protection
	- contributor protection
	- opensource
-   dependency management: dependabot (and alternatives - renovate)
-   advanced security (and alternatives - gitguardian)
-   github RBAC model

--

<!-- slide bg="#157394" -->
### What you learned Lab-4

- Setting up workflow on github for your team 
- Setting up open source projects securely
- RBAC management for github across teams in an organisation
- dependency management for code in any language

---

<!-- slide bg="https://images.unsplash.com/photo-1518770660439-4636190af475?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2340&q=80" data-background-opacity="0.3" -->
<!-- slide style="font-size: 30px" -->
## Lab-5

Getting started with pipelines, secrets, environments on git with github actions

-   Build a very basic pipeline for a hello world
-   Build a basic pipeline to execute a test on some code
-   Build a docker image and push to github packages
-   Full continuous deploy a documentation site
-   Any other advanced usecases of continuous cloud deploy
-   Continuous Infrastructure with terraform and github actions

--

<!-- slide bg="#157394" -->
### What you learned Lab-5


---

<!-- slide bg="https://images.unsplash.com/photo-1496065187959-7f07b8353c55?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2340&q=80" data-background-opacity="0.3" -->

## Lab-6

Getting started with github issues, github projects

--

<!-- slide bg="#157394" -->
### What you learned Lab-6

---

<!-- slide bg="https://images.unsplash.com/photo-1517433456452-f9633a875f6f?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2664&q=80" data-background-opacity="0.3" -->
## Lab-7

Exploration of other tools 
- codespaces
- copilot


--

<!-- slide bg="#157394" -->
### What you learned Lab-6

---

<!-- slide bg="https://media.istockphoto.com/id/846845578/photo/word-appendix-written-on-wood-block.jpg?s=612x612&w=0&k=20&c=UIl44tAoCWETNMM71Tsrkef_0ElRWGR9zU3ypE2ydBM=" data-background-opacity="0.3"-->
## Appendix and Reference

---
<!-- slide bg="#157394" -->
### How git works under the skins

A commit consists of

-   commit
-   tree
-   blob
-   annotated tags

--

### example representation
<!-- slide style="font-size: 30px" -->
<!-- slide bg="#157394" -->
- one commit
![[../../Attachments/Pasted image 20230427231056.png|600x200]]
- commits linked with each other
![[../../Attachments/Pasted image 20230427231224.png |600x200]]



note: 
- Each commit in Git is stored as a “blob”. This blob contains information about the author and the commit message. The blob references another blob that lists the files present in the directory at the time and references blobs that record the state of each file.

- Commits are referenced by a SHA-1 hash (a 40-character hexadecimal string).
- Once you have several commits, each commit blob also links to the hash of the previous commit.


--


