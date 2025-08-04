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
   
 ```bash
 git clone https://github.com/AmrAlmari/Git-Practice-AmroALmari.git
 ```
3. Create Python Script
Create a file main.py with:
 ```python
 print("Hello GitHub!")

 ```
Then push:
 ```bash
git add main.py
git commit -m "Add main.py script"
git push origin main
 ```
4. Create and Push Feature Branch
 ```bash
git checkout -b feature/info
echo "My name is Amro Almari. I love AI and coding." > info.txt
git add info.txt
git commit -m "add info.txt"
git push --set-upstream origin feature/info
 ```
Then go to GitHub and create a Pull Request from `feature/info` → `main`.
5. Merge the PR on GitHub.
6. Create and Merge fix/readme Branch
```bash
git checkout main
git pull
git checkout -b fix/readme
echo -e "\n## Task Summary\nThis project demonstrates basic Git & GitHub operations." >> README.md
git add README.md
git commit -m "Update README with task summary"
git push --set-upstream origin fix/readme
```
Then create and merge another Pull Request from `fix/readme` → `main`.
7. Add .gitignore
Create a .gitignore file:
```.gitignore
__pycache__/
*.pyc
```
```bash
git add .gitignore
git commit -m "Add .gitignore to exclude Python cache files"
git push
```
