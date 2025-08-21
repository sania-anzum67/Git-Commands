# Git-Commands
Basic-To-Advance(Git-Commands)
📘 Git Commands Guide

This guide covers the most commonly used Git commands, explained simply and categorized for easier understanding.

🛠️ 1. Git Setup
git config --global user.name "Your Name"
git config --global user.email "your@email.com"


✔️ Sets your Git identity (used in commits).

git config --list


✔️ Shows your current Git configurations.

📂 2. Repository Management
git init


✔️ Initializes a new Git repository in the current folder.

git clone <repository_url>


✔️ Creates a copy of an existing repository.

📌 3. Staging & Committing
git status


✔️ Shows the state of files (modified, staged, untracked).

git add <file>
git add .


✔️ Adds files to staging area (. means all files).

git commit -m "Your message"


✔️ Saves changes to local repository with a message.

🔄 4. Branching & Merging
git branch


✔️ Lists all branches.

git branch <branch_name>


✔️ Creates a new branch.

git checkout <branch_name>


✔️ Switches to another branch.

git merge <branch_name>


✔️ Merges the specified branch into the current branch.

🌍 5. Remote Repositories
git remote -v


✔️ Shows linked remote repositories.

git remote add origin <repository_url>


✔️ Links local repo with a remote GitHub repo.

git push -u origin main


✔️ Pushes local changes to remote main branch.

git pull origin main


✔️ Fetches and merges changes from remote repo.

git fetch


✔️ Downloads changes but does not merge them.

🧹 6. Undoing & Cleaning
git reset <file>


✔️ Removes file from staging area.

git reset --hard


✔️ Discards all changes (use carefully!).

git checkout -- <file>


✔️ Reverts file to last committed version.

🔍 7. History & Logs
git log


✔️ Shows commit history.

git log --oneline


✔️ Shows simplified commit history.

git diff


✔️ Shows changes not yet staged.

git show <commit_id>


✔️ Shows details of a specific commit.

🚀 8. Collaboration Workflow (GitHub Flow)

Clone repository → git clone <url>

Create branch → git checkout -b feature-branch

Make changes & commit → git add . && git commit -m "message"

Push branch → git push origin feature-branch

Create Pull Request on GitHub

Review & merge into main

🗑️ 9. Deleting
git branch -d <branch_name>


✔️ Deletes local branch.

git push origin --delete <branch_name>


✔️ Deletes remote branch.

📦 10. Advanced
git stash


✔️ Temporarily saves changes without committing.

git stash pop


✔️ Restores stashed changes.

git rebase <branch_name>


✔️ Reapplies commits on top of another base branch.

✅ Quick Workflow Example
git init
git add .
git commit -m "First commit"
git branch -M main
git remote add origin https://github.com/username/repo.git
git push -u origin main

