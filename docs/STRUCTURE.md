# Portfolio Project Structure

## 📁 Directory Layout

```
tahir-portfolio/
├── index.html              # Main home page (entry point)
│
├── pages/                  # Additional HTML pages
│   ├── about.html         # About/Experience page
│   ├── projects.html      # Projects showcase
│   └── contact.html       # Contact form
│
├── assets/                # Static assets
│   ├── css/              # Stylesheets
│   │   └── style.css     # Main stylesheet
│   ├── js/               # JavaScript files
│   │   └── script.js     # Main JavaScript
│   └── images/           # Image assets
│       ├── projects/     # Project screenshots
│       ├── icons/        # Icon files
│       └── IMAGE_REQUIREMENTS.txt
│
├── docs/                 # Documentation
│   └── STRUCTURE.md     # This file
│
├── README.md            # Personal profile & introduction
├── .gitignore          # Git ignore rules
└── .editorconfig       # Editor configuration
```

## 🔗 File Path References

### From Root (index.html)
```html
<!-- CSS -->
<link rel="stylesheet" href="assets/css/style.css">

<!-- JavaScript -->
<script src="assets/js/script.js"></script>

<!-- Navigation Links -->
<a href="index.html">Home</a>
<a href="pages/about.html">About</a>
<a href="pages/projects.html">Projects</a>
<a href="pages/contact.html">Contact</a>

<!-- Images -->
<img src="assets/images/profile.jpg">
<img src="assets/images/projects/project-name.jpg">
```

### From Pages Directory (pages/*.html)
```html
<!-- CSS -->
<link rel="stylesheet" href="../assets/css/style.css">

<!-- JavaScript -->
<script src="../assets/js/script.js"></script>

<!-- Navigation Links -->
<a href="../index.html">Home</a>
<a href="about.html">About</a>
<a href="projects.html">Projects</a>
<a href="contact.html">Contact</a>

<!-- Images -->
<img src="../assets/images/profile.jpg">
<img src="../assets/images/projects/project-name.jpg">
```

## 📄 File Descriptions

### HTML Files
- **index.html**: Landing page with hero section and introduction
- **pages/about.html**: Detailed professional experience, skills, and background
- **pages/projects.html**: Portfolio of projects with descriptions and links
- **pages/contact.html**: Contact information and form

### Assets
- **assets/css/style.css**: Custom styles, animations, and responsive design
- **assets/js/script.js**: Interactive features and form validation
- **assets/images/**: All images including profile, projects, and icons

### Documentation
- **README.md**: Personal introduction and professional profile
- **docs/STRUCTURE.md**: Project structure documentation (this file)

### Configuration
- **.gitignore**: Files to exclude from version control
- **.editorconfig**: Code formatting standards

## 🎯 Benefits of This Structure

1. **Simple & Clean**: Straightforward organization easy to navigate
2. **Web-Ready**: Works perfectly with any static hosting (GitHub Pages, Netlify, Vercel)
3. **Scalable**: Easy to add new pages or assets
4. **Professional**: Follows standard web project conventions
5. **Maintainable**: Logical grouping makes updates simple

## 🚀 Deployment

This structure is ready for deployment to:

### GitHub Pages
1. Push code to repository
2. Enable GitHub Pages in settings
3. Site will be live at `https://username.github.io/repo-name/`

### Netlify
1. Drag and drop the entire folder
2. Site deploys instantly
3. Root `index.html` is automatically recognized

### Vercel
1. Connect GitHub repository
2. Deploy with one click
3. Automatic deployments on push

## 📝 Adding Content

### Add New Page
1. Create HTML file in `pages/` directory
2. Use this template for navigation:
```html
<!-- CSS Link -->
<link rel="stylesheet" href="../assets/css/style.css">

<!-- Navigation -->
<a href="../index.html">Home</a>
<a href="about.html">About</a>
<!-- Add your new page link -->

<!-- JavaScript -->
<script src="../assets/js/script.js"></script>
```

### Add New Image
1. Place image in appropriate subdirectory:
   - Profile photos: `assets/images/`
   - Project screenshots: `assets/images/projects/`
   - Icons: `assets/images/icons/`
2. Reference in HTML:
```html
<!-- From root -->
<img src="assets/images/projects/my-project.jpg">

<!-- From pages/ -->
<img src="../assets/images/projects/my-project.jpg">
```

### Modify Styles
1. Edit `assets/css/style.css`
2. Changes apply to all pages automatically
3. Use CSS variables for easy theme customization:
```css
:root {
    --primary-color: #6366f1;
    --secondary-color: #8b5cf6;
    /* Add your colors here */
}
```

## 🔧 Local Development

### Using Python
```bash
# From project root
python3 -m http.server 8000

# Open browser to http://localhost:8000
```

### Using Node.js
```bash
# Install http-server globally
npm install -g http-server

# Run from project root
http-server

# Open browser to http://localhost:8080
```

### Using VS Code
1. Install "Live Server" extension
2. Right-click `index.html`
3. Select "Open with Live Server"

## ✅ Structure Validation

Use this checklist to verify your structure:

- [ ] `index.html` at root level
- [ ] All pages in `pages/` directory
- [ ] CSS file at `assets/css/style.css`
- [ ] JavaScript at `assets/js/script.js`
- [ ] Images in `assets/images/` subdirectories
- [ ] All navigation links use correct relative paths
- [ ] CSS and JS references work from all pages
- [ ] No broken links or missing files

## 🎨 Customization Guide

### Colors
Edit `assets/css/style.css`:
```css
:root {
    --primary-color: #6366f1;      /* Your brand color */
    --secondary-color: #8b5cf6;    /* Accent color */
    --dark-bg: #0f172a;            /* Background */
}
```

### Fonts
Current fonts (Google Fonts):
- Poppins: Body text
- Playfair Display: Headings

To change, update the `<link>` tag in HTML files and CSS:
```css
body {
    font-family: 'Your-Font', sans-serif;
}
```

### Layout
Modify Bootstrap classes or custom CSS:
- Grid system: `.container`, `.row`, `.col-*`
- Spacing: `.mb-*`, `.mt-*`, `.p-*`, `.m-*`
- Display: `.d-flex`, `.align-items-center`, etc.

## 📞 Need Help?

If you encounter issues:
1. Check browser console for errors (F12)
2. Verify all file paths are correct
3. Ensure local server is running for testing
4. Check that CSS/JS files are being loaded (Network tab in DevTools)

---

**Last Updated**: 2025-11-25
**Version**: 2.0 - Simplified Structure
