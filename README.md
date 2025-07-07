<div align="center">

# 🧰 Git & GitHub Commands Cheat Sheet for Beginners

</div>

Welcome! This repo is designed for beginners learning Git and GitHub. It includes essential commands, real examples, common errors, and extra tips to help you get comfortable with version control.

---

<div align="center">

## 📁 Getting Started

</div>

### 1. Initialize a Git Repository

```bash
mkdir my-website
cd my-website
git init
```

### 2. Clone an Existing Repository

```bash
git clone https://github.com/username/repo-name.git
```

---

## 📝 Working with Files

### 3. Check Status

```bash
git status
```

### 4. Add Files to Staging

```bash
git add index.html       # Add specific file
git add .                # Add all changes
```

### 5. Commit Changes

```bash
git commit -m "Add homepage"
```

---

### 🔄 6. Check Commit History

```bash
git log              # View full history
git log --oneline    # Condensed view
```

### 🚚 7. Rename or Move Files

```bash
git mv oldname.txt newname.txt
```

### 🔍 8. View File Changes

```bash
git diff             # View unstaged changes
git diff --staged    # View staged changes
git diff HEAD        # Compare working directory with last commit
```

---

<div align="center">

## 🗑️ Working with Remotes

</div>

### 9. Add Remote Origin

```bash
git remote add origin https://github.com/username/my-repo.git
```

### 10. Push Changes

```bash
git push -u origin main
```

### 11. Pull Updates

```bash
git pull origin main
```

---

<div align="center">

## 🌿 Branching and Merging

</div>

### 12. Create and Switch Branch

```bash
git checkout -b feature-login
```

### 13. Merge a Branch

```bash
git checkout main
git merge feature-login
```

---

<div align="center">

## 🛠️ Fixing Mistakes

</div>

### 14. Undo Last Commit (keep changes)

```bash
git reset --soft HEAD~1
```

### 15. Discard Changes

```bash
git checkout -- about.html
```

### 16. Remove Untracked Files

```bash
git clean -fd
```

---

### 💾 17. Stash Changes (Temporarily Save Work)

```bash
git stash         # Save current changes
git stash list    # List stashes
git stash apply   # Reapply latest stash
```

---

<div align="center">

## ⚙️ Configuration

</div>

### 18. Set Git User Info

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

---

<div align="center">

## 🔐 HTTPS vs SSH

</div>

### 19. Quick Guide

- **HTTPS:** Easier to set up, ask for credentials/token.
- **SSH:** More secure, needs key setup.

```bash
# Check if SSH is working
ssh -T git@github.com
```

[GitHub SSH Setup Guide](https://docs.github.com/en/authentication/connecting-to-github-with-ssh)



<div align="center">

---

<div align="center">

## 🏷️ Tagging

</div>

### 20. Tag a Commit

```bash
git tag v1.0
git tag -a v1.0 -m "v1.0 release"
git push origin v1.0
```

---

## ❌ Common Git Errors & Fixes

</div>

**Error:** `fatal: not a git repository`  
**Fix:**

```bash
git init
```

**Error:** `failed to push some refs`  
**Fix:**

```bash
git pull --rebase origin main
git push
```

**Error:** Merge conflict  
**Fix:**

- Edit conflicting files
- Then:

```bash
git add filename
git commit
```

**Error:** Detached HEAD  
**Fix:**

```bash
git checkout main
```

**Error:** Permission denied (publickey)  
**Fix:** [GitHub SSH Setup Guide](https://docs.github.com/en/authentication/connecting-to-github-with-ssh)

---

<div align="center">

## 📚 Helpful Resources

</div>

- [Official Git Documentation](https://git-scm.com/doc)
- [GitHub Docs](https://docs.github.com/)
- [Learn Git Branching (interactive)](https://learngitbranching.js.org/)
- [Oh My Git! (interactive Git game)](https://ohmygit.org/)
- [GitHub Cheat Sheet PDF](https://training.github.com/downloads/github-git-cheat-sheet.pdf)

---

<div align="center">

## 🎨 Basic Git Workflow Diagram

</div>

```
      ┌──────────────┐
      │  git init    │ ← Start repo
      └──────────────┘
           ↓
    ┌────────────────┐
    │  git add .     │ ← Stage changes
    └────────────────┘
           ↓
  ┌───────────────────────┐
  │ git commit -m "msg"   │ ← Save snapshot
  └───────────────────────┘
           ↓
 ┌────────────────────────────┐
 │ git push origin main       │ ← Push to GitHub
 └────────────────────────────┘
```

---

<div align="center">

## 💻 GitHub GUI Tips

</div>

✅ Use **GitHub Desktop** for visual Git operations  
✅ On **GitHub.com**, you can:

- Edit files
- Create branches
- Open pull requests
- Merge via UI

---

<div align="center">

## 🚀 Sample Workflow

</div>

```bash
git init
echo "# My Project" > README.md
git add README.md
git commit -m "Initial commit"
git remote add origin https://github.com/username/my-project.git
git push -u origin main
```

---

<div align="center">

## 💡 Pro Tips

</div>

- Use a `.gitignore` file to skip unwanted files.
- Commit frequently with clear messages.
- Use `git pull --rebase` to avoid extra merge commits.
- Always create feature branches for updates.

---

<div align="center">

## 💬 Contributing

</div>

Pull requests are welcome! If you have useful tips or improvements, feel free to open an issue or submit a PR.

---

## 📝 License

This project is licensed under the [MIT License](https://choosealicense.com/licenses/mit/).

Feel free to use, share, and adapt this content with proper attribution.

---

> *"Version control is not just a tool — it's a mindset."*  
> — **Anonymous**

---
