# 🚀 Quick Setup Guide for Craftizen Website

## Step 1: Add Your Images 📸

You have 4 images to add. Save them in the `images/` folder with these names:

### Image 1: hero.png
- **Source**: The first image you showed me (mugs with yellow background)
- **Location**: Save as `images/hero.png`
- This is your main cover/hero image

### Image 2: qr-code.png  
- **Source**: The second image you showed me (QR code with social links)
- **Location**: Save as `images/qr-code.png`
- This appears in the contact section

### Image 3: logo.png
- **Source**: The fourth image you showed me (black Craftizen text)
- **Location**: Save as `images/logo.png`
- This appears in the navigation and footer

**How to save the images:**
1. Right-click on each image file
2. Choose "Save As" or "Export"
3. Save them in the `images/` folder with the exact names above

---

## Step 2: Add Your Amazon Store Link 🛒

1. Open `index.html` in a text editor
2. Find line 94 (or search for "amazon-card")
3. Replace `href="#"` with your actual Amazon store URL

**Example:**
```html
<!-- Change this: -->
<a href="#" class="shop-card amazon-card">

<!-- To this: -->
<a href="https://www.amazon.co.uk/your-store-url" class="shop-card amazon-card">
```

---

## Step 3: Test Locally 🧪

Open `index.html` in your web browser to see your website!

Or run a local server:
```bash
cd /Users/narbugurung/Documents/personal/craftizen
python3 -m http.server 8000
```
Then visit: http://localhost:8000

---

## Step 4: Deploy to GitHub Pages 🌐

### 4a. Create GitHub Account (if needed)
- Go to https://github.com and sign up

### 4b. Run These Commands:

```bash
# Navigate to your project
cd /Users/narbugurung/Documents/personal/craftizen

# Initialize git
git init

# Add all files
git add .

# Commit
git commit -m "Launch Craftizen website"
```

### 4c. Create Repository on GitHub:
1. Go to https://github.com/new
2. Repository name: `craftizen`
3. Keep it Public
4. Click "Create repository"

### 4d. Push Your Code:
```bash
# Replace YOUR_USERNAME with your GitHub username
git remote add origin https://github.com/YOUR_USERNAME/craftizen.git
git branch -M main
git push -u origin main
```

### 4e. Enable GitHub Pages:
1. Go to your repository on GitHub
2. Click "Settings" tab
3. Click "Pages" in the left sidebar
4. Under "Source", select "main" branch
5. Click "Save"

**🎉 Your site will be live at:** `https://YOUR_USERNAME.github.io/craftizen/`

Wait 2-3 minutes for the first deployment!

---

## Optional Customizations 🎨

### Change Colors
Edit `style.css` lines 12-20:
```css
:root {
    --primary-color: #f4d03f;      /* Yellow */
    --secondary-color: #5e8c61;    /* Green */
    --accent-color: #4a9ff5;       /* Blue */
}
```

### Update Contact Email
Edit `script.js` line 28 to use your email

### Add More Content
Edit `index.html` to add more sections or modify text

---

## What You Get ✨

✅ Modern, responsive design  
✅ Mobile-friendly navigation  
✅ Amazon store link section  
✅ Social media integration (Instagram, TikTok)  
✅ QR code for easy sharing  
✅ Contact form  
✅ Smooth scrolling  
✅ Professional look  

---

## Need Help? 🆘

**Common Issues:**

**Images not showing?**
- Check filenames are exactly: `hero.png`, `logo.png`, `qr-code.png`
- Make sure they're in the `images/` folder

**Website not updating?**
- Hard refresh: Cmd+Shift+R (Mac) or Ctrl+Shift+R (Windows)
- Wait 5-10 minutes after pushing to GitHub

**Git errors?**
- Make sure you created the GitHub repository first
- Check your GitHub username is correct in the URL

---

## Next Steps After Launch 🚀

1. Share your new website: `https://YOUR_USERNAME.github.io/craftizen/`
2. Update your Instagram bio with the link
3. Add the link to your TikTok profile
4. Consider connecting your custom domain: www.craftizen.co.uk

**Custom Domain Setup:**
- Create a file named `CNAME` (no extension)
- Add one line: `www.craftizen.co.uk`
- Push to GitHub
- Update DNS settings at your domain registrar

---

**You're all set! 🎉 Your website will be live in under an hour!**

