# Portfolio Website

This is the repository for my personal portfolio website showcasing my professional experience, skills, and projects.

## 🚀 Tech Stack

- **Frontend**: HTML5, CSS3, JavaScript
- **Styling**: Custom CSS with Google Fonts (Source Code Pro)
- **Icons**: Font Awesome 6.5.2
- **Hosting**: GitHub Pages with custom domain

## 📁 Project Structure

```
portfolio-website/
├── index.html          # Home page
├── about.html          # About me page with experience and skills
├── projects.html       # Projects showcase
├── index.css           # Home page styles
├── about.css           # About page styles
├── projects.css        # Projects page styles
├── CNAME               # Custom domain configuration
├── assets/             # Images, PDFs, and other assets
│   ├── *.png          # Profile and background images
│   └── *.pdf          # Resume and project documentation
└── README.md          # This file
```

## 🛠️ Local Development

### Option 1: Python HTTP Server (Recommended)

The simplest way to test the site locally:

```bash
# Navigate to the project directory
cd portfolio-website

# Start the server on port 8000
python3 -m http.server 8000
```

Then open your browser and navigate to:
- **Home**: http://localhost:8000/index.html
- **About**: http://localhost:8000/about.html
- **Projects**: http://localhost:8000/projects.html

**Note**: You need to include `.html` extensions in the URLs when using Python's http.server, as it doesn't support URL rewriting like the production server.

### Option 2: Node.js HTTP Server (with clean URLs)

If you prefer clean URLs without `.html` extensions (like in production):

```bash
# Install http-server globally (one-time setup)
npm install -g http-server

# Start the server with HTML extension support
http-server -p 8000 --ext html
```

Then navigate to:
- **Home**: http://localhost:8000/
- **About**: http://localhost:8000/about
- **Projects**: http://localhost:8000/projects

### Option 3: Direct File Opening

You can also open the HTML files directly in your browser:

```bash
# macOS
open about.html
open projects.html

# Linux
xdg-open about.html

# Windows
start about.html
```

**Note**: Some features may not work correctly when opening files directly (file:// protocol) due to browser security restrictions.

## 🌐 Production Deployment

The site is automatically deployed via GitHub Pages with a custom domain.

**Live URL**: https://ansonwan.com

### Deployment Process

1. Make your changes locally
2. Test using one of the local development methods above
3. Commit your changes:
   ```bash
   git add .
   git commit -m "Update portfolio content"
   ```
4. Push to GitHub:
   ```bash
   git push origin main
   ```
5. GitHub Pages will automatically rebuild and deploy (usually takes 1-2 minutes)
6. Verify changes at https://ansonwan.com

## 📝 Making Updates

### Updating Content
- **About Page**: Edit `about.html` to update experience, skills, or bio
- **Projects**: Edit `projects.html` to add/remove projects
- **Home Page**: Edit `index.html` for landing page changes

### Updating Styles
- Modify `about.css`, `projects.css`, or `index.css` for styling changes

### Updating Resume
- Replace `assets/anson_wan_resume.pdf` with your updated resume
- Update the resume link in navigation if filename changes

## 🎨 Customization

- **Colors & Fonts**: Modify the CSS files (index.css, about.css, projects.css)
- **Content**: Update the HTML files
- **Images**: Add new images to the `assets/` directory
- **Domain**: Update `CNAME` file if changing custom domain

## 📄 License

© 2026 Anson Wan. All rights reserved.