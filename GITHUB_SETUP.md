# GitHub Setup Guide

This guide will help you upload the Linear Theory Calculator project to your GitHub repository.

## 📋 Prerequisites

1. **Git installed** on your computer
2. **GitHub account** (you already have: @princeraj620)
3. **GitHub CLI** (optional, but recommended)

## 🚀 Step-by-Step Upload Process

### Step 1: Create a New Repository on GitHub

1. Go to [GitHub.com](https://github.com) and sign in
2. Click the **"+"** icon in the top right corner
3. Select **"New repository"**
4. Fill in the details:
   - **Repository name**: `linear-theory-calculator`
   - **Description**: `A modern, interactive web application for analyzing network flow systems using linear theory algorithms`
   - **Visibility**: Public (recommended)
   - **Initialize with**: Don't check any boxes (we'll upload existing files)
5. Click **"Create repository"**

### Step 2: Initialize Git in Your Local Project

Open your terminal/command prompt and navigate to your project folder:

```bash
cd "C:\Users\princ\OneDrive\Desktop\hiii"
```

Initialize Git repository:

```bash
git init
```

### Step 3: Add Your Files to Git

Add all files to Git:

```bash
git add .
```

### Step 4: Make Your First Commit

```bash
git commit -m "Initial commit: Linear Theory Calculator v1.0.0"
```

### Step 5: Connect to Your GitHub Repository

Add the remote repository:

```bash
git remote add origin https://github.com/princeraj620/linear-theory-calculator.git
```

### Step 6: Push to GitHub

Push your code to GitHub:

```bash
git branch -M main
git push -u origin main
```

## 🔧 Alternative: Using GitHub CLI

If you have GitHub CLI installed:

```bash
# Login to GitHub
gh auth login

# Create repository and push
gh repo create linear-theory-calculator --public --source=. --remote=origin --push
```

## 🌐 Enable GitHub Pages

After uploading, enable GitHub Pages:

1. Go to your repository on GitHub
2. Click **"Settings"** tab
3. Scroll down to **"Pages"** section
4. Under **"Source"**, select **"Deploy from a branch"**
5. Choose **"main"** branch and **"/ (root)"** folder
6. Click **"Save"**

Your site will be available at: `https://princeraj620.github.io/linear-theory-calculator/`

## 📁 Verify Your Upload

Check that all these files are in your repository:

- ✅ `linear theory algorithm.html` - Main application
- ✅ `index.html` - Entry point
- ✅ `README.md` - Project documentation
- ✅ `LICENSE` - MIT License
- ✅ `package.json` - Project metadata
- ✅ `.gitignore` - Git ignore rules
- ✅ `CONTRIBUTING.md` - Contributing guidelines
- ✅ `CHANGELOG.md` - Version history
- ✅ `SECURITY.md` - Security policy
- ✅ `DEPLOYMENT.md` - Deployment guide
- ✅ `.github/workflows/deploy.yml` - GitHub Actions

## 🎯 Repository Settings

### Enable Issues and Discussions

1. Go to repository **Settings**
2. Scroll down to **"Features"** section
3. Enable:
   - ✅ Issues
   - ✅ Discussions
   - ✅ Wiki (optional)

### Add Repository Topics

Add these topics to your repository:
- `linear-theory`
- `fluid-dynamics`
- `network-analysis`
- `calculator`
- `web-app`
- `javascript`
- `html5`
- `css3`
- `engineering`
- `mathematics`

## 📊 Repository Statistics

After a few days, you should see:
- Repository views
- Clone/download counts
- Star count (hopefully!)
- Fork count

## 🔄 Updating Your Repository

For future updates:

```bash
# Make your changes
# Then commit and push
git add .
git commit -m "Update: brief description of changes"
git push
```

## 🎉 Congratulations!

Your Linear Theory Calculator is now live on GitHub! 

### Next Steps:

1. **Share your repository** on social media
2. **Add to your portfolio** on GitHub profile
3. **Create a demo video** showcasing the features
4. **Write a blog post** about the project
5. **Submit to GitHub trending** repositories

### Useful Links:

- **Live Demo**: https://princeraj620.github.io/linear-theory-calculator/
- **Repository**: https://github.com/princeraj620/linear-theory-calculator
- **Issues**: https://github.com/princeraj620/linear-theory-calculator/issues

---

Happy coding! 🚀 