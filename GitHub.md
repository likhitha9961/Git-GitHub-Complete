# 🐙 GitHub: A Beginner-Friendly Guide  

GitHub is a **website** that allows developers to **store and manage their code using Git**.  

🌐 [Visit GitHub](https://github.com)  

---

## 📦 What is a Repository?  

- In GitHub, **folders are called repositories** (repos).  
- Repositories are where we **keep our project files and code**.  
- We can view other developers' repositories, **clone them** to our system, and make our own changes.  

---

## 📝 Create a Repository  

1. Create an account on GitHub using your email.  
2. Click on **“New Repository”**.  
3. Give your repository a **name** and (optional) **description**.  
4. Add a `README.md` file to describe:  
   - What the project is about  
   - Information about the repository contents  
5. Click **“Create Repository”**.  

---

## 📄 What is `README.md`?  

- `.md` means **Markdown**.  
- A `README.md` file provides **information about the project**.  
- You can use **basic HTML tags** or **Markdown syntax** to make it look better.  

---

## ✅ Initial Commit  

- When we create a repository, GitHub shows **“Initial Commit”**.  
- This means we have made the **first commit (change)** in the repository.  

---

## ✏️ Editing README.md  

- To make changes in the `README.md` file:  
  1. Click the **Edit (✏️)** symbol on GitHub.  
  2. Make your changes.  
  3. Click **“Commit changes”** to save and update it.  

---

## 💻 Open Repository in VS Code  

- Open **VS Code** and open the folder created from GitHub.  
- Open the terminal in VS Code.  
- Git is accessible inside the VS Code terminal to perform the same commands.  

---

## 🔥 Clone a Repository  

### 🗂️ What is Cloning?  

- **Clone**: Making a **duplicate copy** of a repository from GitHub to your local machine.  
- **Remote**: The GitHub repository (online).  
- **Local**: The files and folders on your computer.  

---

### 📥 Command to Clone  
git clone <GitHub-HTTPS-link>

Example:
git clone https://github.com/username/repo-name.git

✅ This copies the GitHub repo into your local folder.

🔥 Git Status

Shows the current status of files in your local repo.

git status

✅ Untracked: New files that Git doesn’t yet track.

✅ Modified: Files have been changed.

✅ Staged: Files are ready to be committed (added but not yet committed).

✅ Unmodified: No changes in the file.

🎨 Stages in Git
| 🗂️ **Stage**  | 📖 **What It Means**                    |
| -------------- | --------------------------------------- |
| **Untracked**  | New file not yet tracked by Git         |
| **Modified**   | File was changed but not staged         |
| **Staged**     | File is added and ready to be committed |
| **Unmodified** | File has no changes                     |

🖥️ Example Workflow

Create or clone a repository.

Make changes to files in VS Code.

Run git status to check file changes.

Add files:
git add <filename>

Commit changes:
git commit -m "Your commit message"

Push to GitHub:
git push origin main