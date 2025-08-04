# Git & GitHub Assignment

## Part 1: Theoretical Questions

### 1. What is the difference between Git and GitHub?

**Git** is a distributed version control system for tracking changes in source code during software development. It is designed for coordinating work among programmers, but it can be used to track changes in any set of files. Its goals include speed, data integrity, and support for distributed, non-linear workflows.

**GitHub** is a web-based Git repository hosting service, which offers all of the distributed revision control and source code management (SCM) functionality of Git as well as adding its own features. 

---

### 2. Explain the difference between `git pull` and `git fetch`.

- `git fetch` downloads the changes from the remote repository to the local repository but does not make any changes to the current working directory.

- `git pull` The git pull command combines `git fetch` and `git merge` (or `git rebase`) into a single command. This allows you to fetch changes from the remote repository and automatically integrate them into the current local branch.

---

### 3. What is the purpose of `.gitignore` file?

The `.gitignore` file specifies which files and directories Git should ignore. Common use cases include ignoring temporary files, logs, and compiled code like `__pycache__/` or `.env`.

---

### 4. Describe the steps to contribute to an open-source project on GitHub.

1. Create the Repository
- Go to Github -> New repository -> Name it: Git-Practice-AmroAlmari
- Check "Add a README file"
  
2. Clone the repo loacally
   
 ```bash git clone https://github.com/AmrAlmari/Git-Practice-AmroALmari.git```

4. Clone the forked repo to your local machine.
5. Create a new branch for your changes.
6. Make your changes and commit them.
7. Push the branch to your GitHub fork.
8. Open a Pull Request to the original repo.
9. Discuss and improve your changes as needed, then get them merged.
