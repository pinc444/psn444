# Personal Portfolio Website

A modern, responsive personal portfolio website designed to be hosted on GitHub Pages with custom domain support.

## Features

- 🎨 Modern purple/blue gradient design
- 📱 Fully responsive (mobile-first approach)
- ⚡ Fast loading with no external dependencies
- 🔗 Social media links section
- 💼 Project showcase grid
- 🌐 Custom domain support via CNAME

## Quick Start

### 1. Fork or Clone This Repository

```bash
git clone https://github.com/yourusername/your-repo-name.git
```

### 2. Customize Your Content

Edit `index.html` to update:
- Your name and tagline in the header
- About me section content
- Social media links (GitHub, LinkedIn, Twitter, Email)
- Project cards with your actual projects

### 3. Enable GitHub Pages

1. Go to your repository on GitHub
2. Navigate to **Settings** → **Pages**
3. Under "Source", select **Deploy from a branch**
4. Choose the **main** branch and **/ (root)** folder
5. Click **Save**

Your site will be live at `https://yourusername.github.io/your-repo-name/` within a few minutes.

## Custom Domain Setup

### Option 1: Apex Domain (yourdomain.com)

1. Update the `CNAME` file with your domain:
   ```
   yourdomain.com
   ```

2. Configure DNS with your domain registrar:
   - Add **A records** pointing to GitHub Pages IP addresses:
     ```
     185.199.108.153
     185.199.109.153
     185.199.110.153
     185.199.111.153
     ```

3. (Optional) Add a **CNAME record** for `www`:
   ```
   www  →  yourusername.github.io
   ```

### Option 2: Subdomain (www.yourdomain.com or blog.yourdomain.com)

1. Update the `CNAME` file with your subdomain:
   ```
   www.yourdomain.com
   ```

2. Configure DNS with your domain registrar:
   - Add a **CNAME record**:
     ```
     www  →  yourusername.github.io
     ```
   - Or for other subdomains:
     ```
     blog  →  yourusername.github.io
     ```

### Verify Custom Domain

1. Go to your repository **Settings** → **Pages**
2. Under "Custom domain", enter your domain
3. Click **Save**
4. Wait for DNS propagation (can take up to 24-48 hours)
5. Enable **Enforce HTTPS** once verification is complete

## Customization Guide

### Changing Colors

The main color scheme is defined in `style.css`. The gradient uses:
- Primary: `#667eea` (purple-blue)
- Secondary: `#764ba2` (purple)

Search for these values in `style.css` to customize the color scheme.

### Adding More Projects

Copy and paste a project card in `index.html`:

```html
<article class="project-card">
    <h3>Project Name</h3>
    <p>Description of your project.</p>
    <a href="https://link-to-project.com" class="project-link">View Project →</a>
</article>
```

### Adding More Social Links

Add a new link in the social-links section:

```html
<a href="https://your-link.com" class="social-link" target="_blank" rel="noopener noreferrer">
    <span class="social-icon">🔗</span>
    <span>Platform Name</span>
</a>
```

## File Structure

```
├── index.html    # Main HTML file
├── style.css     # Stylesheet
├── CNAME         # Custom domain configuration
├── README.md     # This file
└── LICENSE       # MIT License
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome for Android)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Made with ❤️ for the developer community
