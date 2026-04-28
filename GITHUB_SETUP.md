# GitHub Setup Instructions

Follow these steps to upload your portfolio to GitHub and enable GitHub Pages hosting.

## Step 1: Create a GitHub Repository

1. Go to [GitHub](https://github.com/new)
2. Create a new repository with these settings:
   - **Repository name**: `portfolio` (or any name you prefer)
   - **Description**: "Data Engineering Portfolio - Interactive Holographic Design"
   - **Visibility**: Public (required for free GitHub Pages)
   - **Initialize repository**: Leave unchecked (we already have a local repo)

3. Click "Create repository"

## Step 2: Add Remote and Push

Copy and run these commands in your terminal (replace `USERNAME` with your GitHub username):

```bash
git remote add origin https://github.com/USERNAME/portfolio.git
git branch -M main
git push -u origin main
```

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** (top right)
3. Click **Pages** (left sidebar)
4. Under "Build and deployment":
   - **Source**: Select "GitHub Actions"
   - The workflow we created will automatically handle deployment

5. Wait 1-2 minutes for the build to complete

## Step 4: Verify Deployment

1. Go to **Actions** tab in your repository
2. You should see "Deploy Portfolio to GitHub Pages" workflow running
3. Once it's green (✅), your portfolio is live!
4. Visit: `https://USERNAME.github.io/portfolio`

### If using a different repository name:
- Visit: `https://USERNAME.github.io/REPO_NAME`

## Step 5: Update Links (Optional)

If you want the portfolio to be your main profile page:

1. Create a repository named: `USERNAME.github.io` (where USERNAME is your GitHub username)
2. The portfolio will then be available at: `https://USERNAME.github.io`

## Troubleshooting

### Build failed?
- Check the **Actions** tab for error logs
- Ensure the `.github/workflows/deploy.yml` file is correct
- Make sure all files are committed and pushed

### Page not showing?
- GitHub Pages can take up to 5 minutes to deploy
- Clear browser cache (Ctrl+Shift+Delete)
- Verify the repository is public

### Custom domain?
- Go to **Settings > Pages**
- Add your custom domain under "Custom domain"
- Follow the DNS configuration steps

## Files Included

- `index.html` - Main portfolio page with all content
- `README.md` - Portfolio documentation
- `.gitignore` - Git ignore rules
- `.github/workflows/deploy.yml` - GitHub Actions workflow
- `GITHUB_SETUP.md` - This setup guide

## Need Help?

- GitHub Pages Help: https://docs.github.com/en/pages
- GitHub Actions Docs: https://docs.github.com/en/actions

---

Good luck with your portfolio! 🚀
