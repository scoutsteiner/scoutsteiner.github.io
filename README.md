# Byte-Scribe Website

A professional, multi-page website for Byte-Scribe IT Services in Lehigh Valley, PA.

## 🌐 Live Demo

Once deployed to GitHub Pages, your site will be available at:
`https://[your-username].github.io/byte-scribe-website/`

## 📁 Project Structure

```
byte-scribe-website/
├── index.html          # Homepage
├── services.html       # Services page (Business & Residential)
├── about.html          # About Us page
├── contact.html        # Contact page with form
├── css/
│   └── styles.css      # Shared stylesheet
├── js/
│   └── main.js         # JavaScript for mobile menu and navigation
└── images/             # (Optional) Add your images here
```

## 🚀 Deploying to GitHub Pages

### Method 1: Using GitHub Web Interface

1. **Create a new repository on GitHub:**
   - Go to https://github.com/new
   - Repository name: `byte-scribe-website` (or any name you prefer)
   - Make it public
   - Don't initialize with README (we already have files)
   - Click "Create repository"

2. **Upload your files:**
   - Click "uploading an existing file"
   - Drag and drop ALL files and folders from the `byte-scribe-website` folder
   - Commit the changes

3. **Enable GitHub Pages:**
   - Go to repository Settings
   - Scroll down to "Pages" in the left sidebar
   - Under "Source", select "Deploy from a branch"
   - Select branch: `main` (or `master`)
   - Select folder: `/ (root)`
   - Click "Save"

4. **Access your site:**
   - Wait 1-2 minutes for deployment
   - Your site will be live at: `https://[your-username].github.io/byte-scribe-website/`

### Method 2: Using Git Command Line

```bash
# Navigate to the byte-scribe-website folder
cd byte-scribe-website

# Initialize git repository
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit: Byte-Scribe website"

# Add your GitHub repository as remote
git remote add origin https://github.com/[your-username]/byte-scribe-website.git

# Push to GitHub
git branch -M main
git push -u origin main

# Then enable GitHub Pages in repository settings (see Method 1, step 3)
```

## 📝 Customization Guide

### Update Contact Information

Replace placeholder contact details throughout the site:
- Phone: `(610) 555-0123` → Your actual phone
- Email: `support@byte-scribe.com` → Your actual email
- Service areas: Update cities in footer and contact page

### Add Your Logo

1. Create an `images` folder
2. Add your logo image (e.g., `logo.png`)
3. In each HTML file, replace the SVG logo with:
   ```html
   <img src="images/logo.png" alt="Byte-Scribe Logo" class="w-10 h-10">
   ```

### Connect Contact Form to Backend

The contact form currently shows a success message without sending data. To make it functional:

**Option 1: Use Formspree (Easy, Free)**
```html
<!-- In contact.html, update the form tag: -->
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

**Option 2: Use Netlify Forms**
```html
<!-- Add to form tag: -->
<form name="contact" method="POST" data-netlify="true">
```

**Option 3: Build Custom Backend**
- Set up a server with Node.js, PHP, or Python
- Create an API endpoint to receive form submissions
- Update the JavaScript in `contact.html` to POST to your endpoint

### Update Colors

Edit `css/styles.css` to change the color scheme:
```css
:root {
    --blue-600: #2563eb;    /* Primary blue */
    --cyan-400: #22d3ee;    /* Accent cyan */
    --amber-400: #fbbf24;   /* Accent amber */
}
```

### Add Google Analytics

Add this before the closing `</head>` tag in all HTML files:
```html
<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

## 🎨 Features

- ✅ Fully responsive design (mobile, tablet, desktop)
- ✅ Modern animations and transitions
- ✅ SEO-optimized structure
- ✅ Distinct Business vs. Residential service tracks
- ✅ Local SEO focus on Lehigh Valley
- ✅ Professional color scheme
- ✅ Fast loading (CDN-based Tailwind CSS)
- ✅ Accessible navigation with mobile menu
- ✅ Contact form with service type pre-selection

## 🛠️ Tech Stack

- **HTML5** - Semantic markup
- **CSS3** - Custom animations and styles
- **Tailwind CSS** - Utility-first CSS framework (via CDN)
- **JavaScript** - Mobile menu and form handling
- **Google Fonts** - Bitter (serif) + Work Sans (sans-serif)

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 🔧 Local Development

To test locally before deploying:

1. Simply open `index.html` in your web browser
2. Or use a local server:
   ```bash
   # Python 3
   python -m http.server 8000
   
   # PHP
   php -S localhost:8000
   
   # Node.js (with http-server)
   npx http-server
   ```
3. Navigate to `http://localhost:8000`

## 📊 SEO Checklist

- [x] Descriptive page titles
- [x] Meta descriptions on all pages
- [x] Semantic HTML structure
- [x] Alt text for icons (add for images)
- [x] Mobile responsive
- [x] Fast loading times
- [ ] Add sitemap.xml
- [ ] Add robots.txt
- [ ] Submit to Google Search Console
- [ ] Set up Google Business Profile

## 📞 Support

For questions or customization help:
- Email: support@byte-scribe.com (update with your email)
- Phone: (610) 555-0123 (update with your phone)

## 📄 License

© 2026 Byte-Scribe. All rights reserved.

---

**Need help deploying? Contact us and we'll walk you through it!**
