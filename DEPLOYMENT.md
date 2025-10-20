# Deployment Guide

## Option 1: Deploy to Netlify (Recommended - Easiest)

### Method A: Drag & Drop
1. Go to [netlify.com](https://www.netlify.com/)
2. Sign up or log in
3. Drag the entire `portfolio-website` folder onto the Netlify dashboard
4. Your site will be live in seconds!

### Method B: Netlify CLI
```bash
# Install Netlify CLI
npm install -g netlify-cli

# Navigate to project directory
cd portfolio-website

# Deploy
netlify deploy --prod
```

## Option 2: Deploy to Vercel

1. Go to [vercel.com](https://vercel.com/)
2. Sign up or log in
3. Click "Add New Project"
4. Import your Git repository or upload the folder
5. Click "Deploy"

### Vercel CLI
```bash
# Install Vercel CLI
npm install -g vercel

# Navigate to project directory
cd portfolio-website

# Deploy
vercel --prod
```

## Option 3: Deploy to GitHub Pages

1. Create a new repository on GitHub
2. Push your code:
```bash
cd portfolio-website
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin <your-repo-url>
git push -u origin main
```
3. Go to repository Settings > Pages
4. Select source: Deploy from branch `main`
5. Click Save

## Option 4: Deploy to Surge

```bash
# Install Surge
npm install -g surge

# Navigate to project directory
cd portfolio-website

# Deploy
surge
```

## Custom Domain

After deployment, you can add a custom domain in your hosting platform's settings.

### Example Custom Domains:
- `shivampawar.com`
- `shivampawar.dev`
- `yourname.netlify.app` (free subdomain)

## Post-Deployment Checklist

- ✅ Test all links and navigation
- ✅ Verify mobile responsiveness
- ✅ Check contact form functionality
- ✅ Test on different browsers
- ✅ Verify social media links
- ✅ Add custom domain (optional)
- ✅ Set up analytics (Google Analytics, optional)

## Environment Variables (if needed)

If you want to add backend functionality (like email for contact form):
1. Sign up for a service like [EmailJS](https://www.emailjs.com/) or [Formspree](https://formspree.io/)
2. Add the API keys to your hosting platform's environment variables
3. Update the contact form JavaScript

## SSL Certificate

All mentioned hosting platforms (Netlify, Vercel, GitHub Pages, Surge) provide free SSL certificates automatically!
