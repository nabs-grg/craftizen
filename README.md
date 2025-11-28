# Craftizen Website

A beautiful, responsive website for Craftizen - Make every occasion memorable one mug at a time.

## Features

- ✨ Modern, responsive design
- 🎨 Smooth scrolling navigation
- 📱 Mobile-friendly with hamburger menu
- 🛍️ Amazon link section for product sales
- 📸 Instagram integration
- 📧 Contact form
- 🎯 Social media links (Instagram, TikTok, Website)

## Setup Instructions

### 1. Add Your Images

Place the following images in the `images/` folder:

- `hero.png` - Your cover/hero image (the mug display image)
- `logo.png` - Your Craftizen logo
- `qr-code.png` - The QR code image for social connections

### 2. Update Amazon Link

Edit `index.html` and find the Amazon card section (around line 94). Update the `href="#"` with your actual Amazon store URL:

```html
<a href="YOUR_AMAZON_STORE_URL_HERE" class="shop-card amazon-card">
```

### 3. Customize Contact Email (Optional)

In `script.js`, line 28, update the email address:

```javascript
const mailtoLink = `mailto:YOUR_EMAIL@craftizen.co.uk?subject=...`;
```

## Deployment to GitHub Pages

### Step 1: Initialize Git Repository

```bash
cd /Users/narbugurung/Documents/personal/craftizen
git init
git add .
git commit -m "Initial commit - Craftizen website"
```

### Step 2: Create GitHub Repository

1. Go to [GitHub](https://github.com) and log in
2. Click the "+" icon in the top right and select "New repository"
3. Name it `craftizen` (or any name you prefer)
4. **Do NOT** initialize with README, .gitignore, or license
5. Click "Create repository"

### Step 3: Push to GitHub

```bash
git remote add origin https://github.com/YOUR_USERNAME/craftizen.git
git branch -M main
git push -u origin main
```

### Step 4: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings" tab
3. Scroll down to "Pages" in the left sidebar
4. Under "Source", select "main" branch
5. Click "Save"
6. Your site will be live at: `https://YOUR_USERNAME.github.io/craftizen/`

## Local Testing

To test your website locally:

1. Simply open `index.html` in your web browser
2. Or use a local server:

```bash
# If you have Python installed:
python -m http.server 8000

# Then visit http://localhost:8000 in your browser
```

## Customization Tips

### Colors

Edit the CSS variables in `style.css` (lines 12-20) to change the color scheme:

```css
:root {
    --primary-color: #f4d03f;
    --secondary-color: #5e8c61;
    --accent-color: #4a9ff5;
    /* ... */
}
```

### Content

- Edit `index.html` to update text content
- Modify sections, add or remove content as needed
- All text is easily editable in the HTML file

### Adding More Products

You can add more shop cards in the `#shop` section by copying the existing card structure.

## Technologies Used

- HTML5
- CSS3 (with CSS Grid and Flexbox)
- Vanilla JavaScript
- Google Fonts (Poppins)

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## License

© 2024 Craftizen. All rights reserved.

## Support

For questions or support, contact us through:
- Website: www.craftizen.co.uk
- Instagram: @craftizen_uk
- TikTok: @craftizen_uk

---

Made with ❤️ in London, UK

