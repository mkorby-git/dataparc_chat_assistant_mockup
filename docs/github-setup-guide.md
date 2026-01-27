# GitHub Setup Guide - Step-by-Step Reference

## 1. Create a GitHub Repository
- Go to [github.com](https://github.com) and sign in
- Click **"New repository"**
- Name your repository
- Set visibility to **Public**
- Click **Create repository**

---

## 2. Initialize Local Git Repository
```powershell
cd "path\to\your\project"
git init
```

---

## 3. Stage and Commit Your Files
```powershell
git add .
git commit -m "Initial commit"
```

---

## 4. Set Branch to Main
```powershell
git branch -M main
```

---

## 5. Connect to GitHub Remote
```powershell
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
```

**If you made a mistake:**
```powershell
git remote remove origin
git remote add origin https://github.com/CORRECT_URL.git
```

---

## 6. Push Code to GitHub
```powershell
git push -u origin main
```

**If rejected (remote has files you don't have locally):**
```powershell
git pull origin main --allow-unrelated-histories
git push -u origin main
```

---

## 7. Enable GitHub Pages (Free Hosting)
1. Go to your repo on GitHub
2. Click **Settings** → **Pages**
3. Under **Source**, select **main** branch, **/ (root)** folder
4. Click **Save**
5. Site will be at: `https://USERNAME.github.io/REPO_NAME/`

---

## 8. Ensure index.html is Served (Not README)
Create a `.nojekyll` file in your repo root:
```powershell
New-Item -Path ".nojekyll" -ItemType File
git add .nojekyll
git commit -m "Add .nojekyll to serve index.html"
git push
```

---

## 9. Future Updates
After making changes to your files:
```powershell
git add .
git commit -m "Description of changes"
git push
```

---

## Quick Reference - Common Commands

| Command | Purpose |
|---------|---------|
| `git status` | Check current state |
| `git add .` | Stage all changes |
| `git commit -m "message"` | Commit with message |
| `git push` | Push to GitHub |
| `git pull` | Pull latest from GitHub |
| `git remote -v` | View connected remotes |
