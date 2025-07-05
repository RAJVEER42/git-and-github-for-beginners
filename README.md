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

<div align="center">

## 🗑️ Working with Remotes

</div>

### 6. Add Remote Origin

```bash
git remote add origin https://github.com/username/my-repo.git
```

### 7. Push Changes

```bash
git push -u origin main
```

### 8. Pull Updates

```bash
git pull origin main
```

---

<div align="center">

## 🌿 Branching and Merging

</div>

### 9. Create and Switch Branch

```bash
git checkout -b feature-login
```

### 10. Merge a Branch

```bash
git checkout main
git merge feature-login
```

---

<div align="center">

## 🛠️ Fixing Mistakes

</div>

### 11. Undo Last Commit (keep changes)

```bash
git reset --soft HEAD~1
```

### 12. Discard Changes

```bash
git checkout -- about.html
```

### 13. Remove Untracked Files

```bash
git clean -fd
```

---

<div align="center">

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

* Edit file to resolve conflict
  Then:

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
**Fix:**
Set up SSH: [GitHub SSH Setup Guide](https://docs.github.com/en/authentication/connecting-to-github-with-ssh)

---

<div align="center">

## 📚 Helpful Resources

</div>

* [Official Git Documentation](https://git-scm.com/doc)
* [GitHub Docs](https://docs.github.com/)
* [Learn Git Branching (interactive)](https://learngitbranching.js.org/)

---

<div align="center">

## 🎨 Basic Git Workflow Diagram

</div>

```
      ┌──────────┐
      │  git init  │ ← Start repo
      └────────--┘
           ↓
    ┌───────────────┐
    │  git add .    │ ← Stage changes
    └──────────────-┘
         ↓
  ┌────────────────────┐
  │ git commit -m "" │ ← Save changes
  └─────────────────---┘
        ↓
 ┌─────────────────────────┐
 │ git push origin main│ ← Upload to GitHub
 └─────────────────────────┘
```

---

<div align="center">

## 💻 GitHub GUI Tips

</div>

Not comfortable with the terminal?

✅ Use **GitHub Desktop** to commit, push, pull, and merge with a GUI.

✅ On **GitHub.com** you can:

* Edit files directly in-browser
* Create branches
* Open and manage pull requests

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

## 💬 Contributing

</div>

Pull requests are welcome! If you have useful tips or improvements, feel free to open an issue or submit a PR.

---

---

## 📝 License

This project is licensed under the [MIT License](https://choosealicense.com/licenses/mit/).

Feel free to use, share, and adapt this content with proper attribution.

---
