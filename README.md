# Git Cheatsheet (Common Git Commands)

## **Git Overview**
Git is a distributed version control system used for tracking changes in source code during software development.

---

## **Git Setup & Configuration**
```sh
git --version                     # Check Git version
git config --global user.name "Your Name"  # Set user name
git config --global user.email "you@example.com"  # Set user email
git config --global core.editor nano  # Set default editor
git config --list                  # List all configured settings
```

---

## **Initializing a Repository**
```sh
git init                           # Initialize a new Git repository
git clone <repo-url>               # Clone an existing repository
git remote add origin <repo-url>   # Add remote repository
```

---

## **Basic Git Commands**
```sh
git status                         # Check status of working directory
git add <file>                     # Stage a specific file
git add .                          # Stage all changes
git commit -m "Your commit message" # Commit staged changes
git push origin main                # Push changes to remote repository
git pull origin main                # Pull latest changes from remote
```

---

## **Branching & Merging**
```sh
git branch                         # List all branches
git branch <branch-name>           # Create a new branch
git checkout <branch-name>         # Switch to a branch
git checkout -b <branch-name>      # Create and switch to a new branch
git merge <branch-name>            # Merge a branch into the current branch
git branch -d <branch-name>        # Delete a branch
```

---

## **Undoing Changes**
```sh
git reset --soft HEAD~1            # Undo last commit but keep changes staged
git reset --mixed HEAD~1           # Undo last commit and unstage changes
git reset --hard HEAD~1            # Undo last commit and discard changes
git checkout -- <file>             # Discard changes in a file
git revert <commit-hash>           # Create a new commit that undoes a previous commit
```

---

## **Working with Remotes**
```sh
git remote -v                      # Show remote URLs
git push origin <branch-name>       # Push branch to remote
git fetch origin                    # Fetch latest changes from remote
git pull origin <branch-name>       # Pull latest changes from remote
```

---

## **Viewing Commit History**
```sh
git log                             # Show commit history
git log --oneline                   # Show condensed commit history
git log --graph --decorate --all    # Show commit history with branches
```

---

## **Stashing Changes**
```sh
git stash                           # Stash uncommitted changes
git stash list                      # List all stashes
git stash apply                     # Apply last stashed changes
git stash drop                      # Remove last stash
```

---

## **Tagging Releases**
```sh
git tag                             # List all tags
git tag -a v1.0 -m "Version 1.0"    # Create an annotated tag
git push origin --tags              # Push tags to remote repository
```

---

## **Git Aliases**
```sh
git config --global alias.co checkout  # Shorten 'checkout' to 'co'
git config --global alias.br branch    # Shorten 'branch' to 'br'
git config --global alias.st status    # Shorten 'status' to 'st'
```

---

## **Useful Git Resources**
- [Git Documentation](https://git-scm.com/doc)
- [GitHub Learning Lab](https://lab.github.com/)
- [Pro Git Book](https://git-scm.com/book/en/v2)

---

This cheatsheet provides a quick reference for common Git commands, branching, merging, and undoing changes. Let me know if you need any modifications!

