# 🚀 Push Your Portfolio to GitHub

## Step 1: Create GitHub Repository

A browser window should have opened to: https://github.com/new

**Fill in the form:**
1. **Repository name**: `portfolio-website` (or any name you prefer)
2. **Description**: `Professional portfolio website showcasing my web and mobile development projects`
3. **Visibility**: ✅ Public (so it can be viewed by everyone)
4. **Initialize repository**: ❌ DO NOT check any boxes (no README, no .gitignore, no license)
5. Click **"Create repository"**

## Step 2: Push Your Code

After creating the repository, GitHub will show you commands. **IGNORE THOSE** and use these instead:

### Copy and run these commands in your terminal:

```bash
cd /tmp/portfolio-website

# Add your GitHub repository as remote (replace YOUR_USERNAME with mepawarshivam)
git remote add origin https://github.com/mepawarshivam/portfolio-website.git

# Push your code to GitHub
git branch -M main
git push -u origin main
```

**Replace `mepawarshivam` with your actual GitHub username if different!**

## Step 3: After Pushing

Once pushed successfully, your repository will be at:
```
https://github.com/mepawarshivam/portfolio-website
```

## Step 4: Deploy with Netlify

Now you can deploy using Netlify in two ways:

### Option A: From GitHub (Recommended)
1. Go to: https://app.netlify.com/start
2. Click "Import from Git"
3. Choose GitHub
4. Select your `portfolio-website` repository
5. Click "Deploy site"
6. **Done!** Your site will be live in seconds

### Option B: Drag & Drop
1. Go to: https://app.netlify.com/drop
2. Drag the `/tmp/portfolio-website` folder
3. **Done!** Instant deployment

## Step 5: Enable GitHub Pages (Optional - Second Deployment)

You can also host on GitHub Pages:
1. Go to your repository: `https://github.com/mepawarshivam/portfolio-website`
2. Click **Settings** → **Pages** (in left sidebar)
3. Under "Source", select branch: **main**
4. Click **Save**
5. Your site will be live at: `https://mepawarshivam.github.io/portfolio-website/`

## Quick Commands Reference

```bash
# Navigate to portfolio
cd /tmp/portfolio-website

# Add remote (use your actual username)
git remote add origin https://github.com/YOUR_USERNAME/portfolio-website.git

# Push to GitHub
git branch -M main
git push -u origin main
```

## Troubleshooting

**If you get an authentication error:**
1. GitHub might ask for credentials
2. Use a Personal Access Token instead of password
3. Generate one at: https://github.com/settings/tokens
4. Or install GitHub CLI: `brew install gh` and run `gh auth login`

**If remote already exists:**
```bash
git remote remove origin
git remote add origin https://github.com/YOUR_USERNAME/portfolio-website.git
git push -u origin main
```

---

## 🎉 Next Steps After GitHub Push

1. ✅ Deploy to Netlify from GitHub
2. ✅ Add repository link to your LinkedIn
3. ✅ Share your live portfolio URL
4. ✅ Keep updating with new projects!

**Your portfolio is ready to go live! 🚀**
