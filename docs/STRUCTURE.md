# Project Structure

This document describes the directory structure and organization of the portfolio website.

## Directory Layout

```
tahir-portfolio/
├── public/                  # Public-facing entry point
│   └── index.html          # Main landing page
│
├── src/                    # Source files
│   ├── assets/            # Static assets
│   │   ├── css/          # Stylesheets
│   │   │   └── style.css # Main stylesheet
│   │   ├── js/           # JavaScript files
│   │   │   └── script.js # Main JavaScript
│   │   ├── images/       # Image assets
│   │   │   ├── projects/ # Project screenshots
│   │   │   ├── icons/    # Icon files
│   │   │   └── IMAGE_REQUIREMENTS.txt
│   │   └── fonts/        # Custom fonts (if any)
│   │
│   ├── pages/            # Additional HTML pages
│   │   ├── about.html    # About page
│   │   ├── projects.html # Projects showcase
│   │   └── contact.html  # Contact form
│   │
│   └── components/       # Reusable components (future use)
│
├── docs/                 # Documentation
│   └── STRUCTURE.md     # This file
│
├── README.md            # Project overview
└── .gitignore          # Git ignore rules

```

## File Organization

### Public Directory
- **Purpose**: Contains the main entry point (index.html) that visitors see first
- **Access**: Files here are directly accessible via web server

### Source Directory
- **Assets**: All static resources organized by type
  - CSS: Stylesheets for visual design
  - JS: Client-side scripts for interactivity
  - Images: Photos, screenshots, and graphics
  - Fonts: Custom typography files
- **Pages**: Additional HTML pages for different sections
- **Components**: Reusable UI components (for future modular development)

### Documentation
- Contains project documentation and guides
- Helps developers understand the codebase structure

## Path References

### From index.html (public/)
- CSS: `../src/assets/css/style.css`
- JS: `../src/assets/js/script.js`
- Pages: `../src/pages/[page-name].html`

### From other pages (src/pages/)
- CSS: `../assets/css/style.css`
- JS: `../assets/js/script.js`
- Home: `../../public/index.html`
- Other pages: `[page-name].html` (same directory)

## Benefits of This Structure

1. **Separation of Concerns**: Assets, pages, and documentation are clearly separated
2. **Scalability**: Easy to add new pages, components, or assets
3. **Maintainability**: Logical organization makes code easier to find and update
4. **Professional Standard**: Follows industry best practices for web projects
5. **Build-Ready**: Structure is compatible with build tools and bundlers

## Future Enhancements

- Add a `config/` directory for configuration files
- Implement component-based architecture in `src/components/`
- Add a `tests/` directory for automated testing
- Include a `build/` or `dist/` directory for production builds
