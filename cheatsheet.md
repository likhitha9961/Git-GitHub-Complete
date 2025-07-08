# 📝 Git Cheat Sheet

Git is a free and open-source **distributed version control system** that allows you to track changes in your projects, collaborate with others, and manage code versions efficiently.  

---

## 🚀 Setup

### Configure User Information
```bash
git config --global user.name "[firstname lastname]"    # Set your name for commits
git config --global user.email "[valid-email]"          # Set your email for commits
git config --global color.ui auto                       # Enable automatic coloring

📁 Setup & Init
Initialize & Clone Repositories

git init                              # Initialize an existing directory as a Git repository
git clone [url]                       # Clone a remote repository to your local machine

🌿 Stage & Snapshot
Working with Snapshots & Staging Area

git status                            # Show modified files in working directory
git add [file]                        # Add file to staging area
git reset [file]                      # Unstage a file (keep changes)
git diff                              # Show changes not staged
git diff --staged                     # Show staged changes
git commit -m "[message]"             # Commit staged changes with message

🌱 Branch & Merge
Isolate Work & Combine Changes

git branch                            # List branches (shows * next to active branch)
git branch [branch-name]              # Create a new branch
git checkout [branch-name]            # Switch to a branch
git checkout -b [branch-name]         # Create and switch to new branch
git merge [branch]                    # Merge a branch into the current branch
git log                               # Show commit history

🌐 Share & Update
Collaborate with Remotes

git remote add [alias] [url]          # Add a Git remote repository
git fetch [alias]                     # Fetch branches from remote
git merge [alias]/[branch]            # Merge remote branch into local branch
git push [alias] [branch]             # Push local commits to remote repository
git pull                              # Fetch and merge remote commits

📂 Tracking Path Changes
Version File Deletes & Moves

git rm [file]                         # Delete file and stage removal
git mv [old-path] [new-path]          # Move or rename a file and stage the change
git log --stat -M                     # Show commit logs including file moves

🛠 Temporary Commits
Work In Progress with Stash

git stash                             # Save modified files temporarily
git stash list                        # Show stashed changes
git stash pop                         # Apply and remove latest stash
git stash drop                        # Discard latest stash

⚡ Rewrite History
Adjust Commits

git rebase [branch]                   # Reapply commits on top of another base branch
git reset --hard [commit]             # Reset branch & working tree to a specific commit

🔍 Inspect & Compare
Examine Changes & History

git log                               # Show commit history
git log branchB..branchA              # Show commits in branchA not in branchB
git log --follow [file]               # Show history of a file (across renames)
git diff branchB...branchA            # Show differences between branches
git show [SHA]                        # Display information about a commit or object

🚫 Ignoring Patterns
Exclude Files from Git

git config --global core.excludesfile [file]   # Set global ignore file

Add patterns in .gitignore:

logs/
*.notes
pattern*/


