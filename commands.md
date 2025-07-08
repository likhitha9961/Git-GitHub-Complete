✍️ Add, Commit & Push

✅ Add

Add files to the staging area:

git add <file-name>

✅ Commit

Save changes to the repository:

git commit -m "your commit message"

🚀 Push

Upload changes from your local repo to GitHub:

git push origin main

🏗️ Initialize a New Repo & Push

1️⃣ Initialize Git in a folder:

git init

2️⃣ Add remote repository:

git remote add origin <repo-link>

3️⃣ Verify remote:

git remote -v

4️⃣ Rename branch to main:

git branch -M main

5️⃣ Push to GitHub:

git push -u origin main

💡 -u: Sets upstream so next time you can just use git push.

🌿 Git Branches

If multiple developers work on different features, use branches.

🛠 Branch Commands

| Command                             | Description                                                |
| ----------------------------------- | ---------------------------------------------------------- |
| `git branch`                        | Check the current branch.                                  |
| `git branch -M main`                | Rename the branch to `main`.                               |
| `git checkout <branch-name>`        | Switch to another branch.                                  |
| `git checkout -b <new-branch-name>` | Create and switch to a new branch.                         |
| `git branch -d <branch-name>`       | Delete a branch (must be on a different branch to delete). |


🔀 Merging Branches

✅ Merge with Commands

Switch to the main branch:


git checkout main

Merge feature branch into main:


git merge <feature-branch>

⚔️ Resolving Merge Conflicts

Merge conflicts happen when two people change the same line of a file.

Git shows:

<<<<<<< HEAD

Your changes here

=======

Their changes here

>>>>>>> feature-branch

✅ Fix conflict, mark resolved:

git add <file>

git commit -m "Resolved merge conflict"

🍴 GitHub Fork

A fork is a copy of someone else’s repository into your GitHub account.

✅ Why Fork?

Experiment safely.

Suggest changes via Pull Requests.

🖇️ Fork Workflow

1️⃣ Click Fork on GitHub.

2️⃣ Clone your fork locally:

git clone <your-fork-link>

3️⃣ Make changes.

4️⃣ Push changes:

git push origin main

5️⃣ Submit a Pull Request to the original repo.

🥊 Merge vs Fork
| 🔀 Merge                          | 🍴 Fork                                 |
| --------------------------------- | --------------------------------------- |
| Combines changes in the same repo | Creates a separate copy in your account |
| Used by team members              | Used when you don’t have write access   |
| Happens locally or on GitHub      | Happens only on GitHub                  |


📝 Quick Commands Reference
| Command                             | Description                                |
| ----------------------------------- | ------------------------------------------ |
| `git init`                          | Initialize a new Git repository.           |
| `git add <file-name>`               | Add file(s) to the staging area.           |
| `git commit -m "message"`           | Commit changes with a message.             |
| `git remote add origin <repo-link>` | Link local repo to GitHub.                 |
| `git push origin main`              | Push changes to GitHub.                    |
| `git checkout -b <branch-name>`     | Create and switch to a new branch.         |
| `git merge <branch-name>`           | Merge branch into current branch.          |
| `git pull origin main`              | Pull changes from GitHub to local machine. |
