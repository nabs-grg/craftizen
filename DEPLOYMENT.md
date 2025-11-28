# Quick Deployment Guide

## Before You Deploy

### 1. Add Your Images
Copy these three images to the `images/` folder:
- `hero.png` (cover image with mugs)
- `logo.png` (Craftizen logo)
- `qr-code.png` (QR code)

### 2. Update Amazon Link
Edit `index.html` line 94 and replace `href="#"` with your Amazon store URL.

## Deploy to GitHub Pages (5 Minutes)

### Quick Commands:

```bash
# 1. Navigate to project folder (if not already there)
cd /Users/narbugurung/Documents/personal/craftizen

# 2. Initialize git (if not done)
git init

# 3. Add all files
git add .

# 4. Commit
git commit -m "Initial Craftizen website"

# 5. Create repository on GitHub first, then:
git remote add origin https://github.com/YOUR_USERNAME/craftizen.git

# 6. Push to GitHub
git branch -M main
git push -u origin main
```

### Enable GitHub Pages:
1. Go to repository Settings
2. Click "Pages" in sidebar
3. Select "main" branch as source
4. Save

**Your site will be live at:** `https://YOUR_USERNAME.github.io/craftizen/`

## Alternative: Deploy to Netlify (Even Easier!)

### Option 1: Drag & Drop
1. Go to [Netlify Drop](https://app.netlify.com/drop)
2. Drag the entire `craftizen` folder
3. Done! You'll get a live URL instantly

### Option 2: Connect to Git
1. Push your code to GitHub (steps above)
2. Go to [Netlify](https://netlify.com)
3. Click "New site from Git"
4. Connect your GitHub repository
5. Deploy!

## Test Locally First

```bash
# Simple Python server
python -m http.server 8000

# Or Python 3
python3 -m http.server 8000

# Then visit: http://localhost:8000
```

## Custom Domain (Optional)

Once deployed, you can connect `www.craftizen.co.uk`:

### GitHub Pages:
1. Add CNAME file with your domain
2. Update DNS settings at your domain registrar

### Netlify:
1. Go to Domain Settings
2. Add custom domain
3. Follow DNS instructions

## Troubleshooting

**Images not showing?**
- Check filenames match exactly (case-sensitive)
- Ensure images are in the `images/` folder

**Site not updating?**
- Clear browser cache (Cmd+Shift+R on Mac)
- Wait 5-10 minutes for GitHub Pages to rebuild
- Check GitHub Actions tab for build status

**Form not working?**
- The contact form uses `mailto:` by default
- For better functionality, consider using [Formspree](https://formspree.io/) (free)

## Need Help?

- GitHub Pages: https://pages.github.com/
- Netlify Docs: https://docs.netlify.com/

