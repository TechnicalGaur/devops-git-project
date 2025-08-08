🚀  Build a Version-Controlled DevOps Project with Git

This repository contains the setup and workflow for devops-git-project using Git, GitHub, and other tools. It includes all the commands and steps used in the process, so anyone can replicate it easily.

📂 Table of Contents
1. Project Overview

2. Prerequisites

3. Step-by-Step Commands

4. Common Git Issues & Fixes

5. Pull Request Workflow

6. License


📜 Project Overview
This project demonstrates:

Initializing a Git repository

Adding and committing files

Creating .gitignore

Connecting to a GitHub repository via SSH & HTTPS

Pushing code to GitHub

Creating branches and merging via Pull Requests


🛠 Prerequisites
Before starting, make sure you have:

Git installed → Download Git

GitHub Account → Create here

SSH key configured for GitHub → Guide





🖥 Step-by-Step Commands

1️⃣ Initialize Git Repository

```git init```

Initializes a new Git repository in your project folder.

2️⃣ Create .gitignore file

```touch .gitignore```
      
Creates a .gitignore file to exclude files/folders from Git tracking.

3️⃣ Check Status of Repository

```git status```

Displays changes in your working directory.

4️⃣ Add Files for Commit

```git add .```

Stages all modified and new files for commit.

5️⃣ Commit Changes

```git commit -m "Your commit message"```

Saves your staged changes into Git history.

6️⃣ Link Local Repo to GitHub (HTTPS)

```git remote add origin https://github.com/username/repo.git```

6️⃣ Link Local Repo to GitHub (SSH)

```git remote add origin git@github.com:username/repo.git```

Connects your local repository to GitHub.

7️⃣ Push Code to GitHub

```git push -u origin main```

Pushes your commits to the main branch of GitHub.

8️⃣ Create a New Branch

```git checkout -b feature-branch```

Creates and switches to a new branch.

9️⃣ Push New Branch to GitHub

```git push origin feature-branch```

Uploads your branch to GitHub for collaboration.

🐞 Common Git Issues & Fixes
❌ Error:

```fatal: pathspec '.gitignore' did not match any files```

✅ Fix:
Make sure .gitignore exists. Create it:

```touch .gitignore```

❌ Error:


```git@github.com: Permission denied (publickey)```

✅ Fix:
Generate SSH key and add to GitHub:

```ssh-keygen -t rsa -b 4096 -C "your_email@example.com"```
```cat ~/.ssh/id_rsa.pub```

Then add the key to GitHub → SSH Settings

🔄 Pull Request Workflow (Without gh pr)

1. Push your branch to GitHub:
   ```git push origin feature-branch```

2.Go to your repository on GitHub in the browser.
3.Click "Compare & pull request".
4.Add title & description.
5.Click "Create pull request".


📄 License
This project is licensed under the MIT License — you are free to use, modify, and share it.





