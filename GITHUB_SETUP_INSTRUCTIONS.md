# GitHub Pages Setup Instructions

Follow these steps to host your OAuth verification pages on GitHub Pages:

## Step 1: Create a GitHub Repository

1. Go to [GitHub.com](https://github.com) and log in to your account
2. Click the "+" icon in the top right corner and select "New repository"
3. Name your repository: `oauth-verification-pages`
4. Make sure to select "Public" (not private)
5. Do NOT initialize with a README
6. Click "Create repository"

## Step 2: Push Your Code to GitHub

After creating the repository, GitHub will show you commands to push an existing repository. 
Run these commands in your terminal (replace `YOUR_USERNAME` with your actual GitHub username):

```bash
git remote add origin https://github.com/YOUR_USERNAME/oauth-verification-pages.git
git branch -M main
git push -u origin main
```

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on "Settings" tab
3. Scroll down to the "Pages" section in the left sidebar
4. Under "Source", select "Deploy from a branch"
5. Select "main" branch and "/ (root)" folder
6. Click "Save"
7. Wait a few minutes for GitHub Pages to build your site

## Step 4: Get Your URLs

After GitHub Pages is enabled, your pages will be available at:
- Homepage: `https://YOUR_USERNAME.github.io/oauth-verification-pages/`
- Privacy Policy: `https://YOUR_USERNAME.github.io/oauth-verification-pages/privacy.html`
- Terms of Service: `https://YOUR_USERNAME.github.io/oauth-verification-pages/terms.html`

## Step 5: Update Your OAuth Consent Screen

1. Go to the Google Cloud Console
2. Select your project
3. Go to "APIs & Services" > "OAuth consent screen"
4. Update the following fields with your new GitHub Pages URLs:
   - Authorized domains: Add `YOUR_USERNAME.github.io`
   - Application homepage: `https://YOUR_USERNAME.github.io/oauth-verification-pages/`
   - Application privacy policy: `https://YOUR_USERNAME.github.io/oauth-verification-pages/privacy.html`
   - Application terms of service: `https://YOUR_USERNAME.github.io/oauth-verification-pages/terms.html`

## Need Help?

If you need any assistance with this process, please reach out for support.