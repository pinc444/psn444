# Personal Website

A modern, responsive personal website template designed to be hosted on GitHub Pages with custom domain support.

## Features

- 🎨 Modern gradient design with purple/blue theme
- 📱 Fully responsive layout for all devices
- ⚡ Fast loading with minimal dependencies
- 🔗 Social links section (GitHub, LinkedIn, Twitter, Email)
- 📦 Project showcase grid
- 🌐 Custom domain support via CNAME

## Quick Start

### Hosting on GitHub Pages

1. **Fork or clone this repository** to your GitHub account

2. **Enable GitHub Pages:**
   - Go to your repository's **Settings**
   - Navigate to **Pages** (under "Code and automation")
   - Under "Source", select **Deploy from a branch**
   - Choose the `main` branch and `/ (root)` folder
   - Click **Save**

3. **Access your site:**
   - Your site will be available at `https://yourusername.github.io/repository-name/`
   - It may take a few minutes for the site to deploy

## Custom Domain Setup

### Option 1: Apex Domain (e.g., `example.com`)

1. **Update the CNAME file:**
   - Replace `yourdomain.com` with your actual domain

2. **Configure DNS with your domain provider:**
   - Add the following **A records** pointing to GitHub Pages:
     ```
     185.199.108.153
     185.199.109.153
     185.199.110.153
     185.199.111.153
     ```

3. **Enable custom domain in GitHub:**
   - Go to repository **Settings** → **Pages**
   - Enter your domain in the "Custom domain" field
   - Check "Enforce HTTPS" (recommended)

### Option 2: Subdomain (e.g., `www.example.com`)

1. **Update the CNAME file:**
   - Replace `yourdomain.com` with your subdomain (e.g., `www.example.com`)

2. **Configure DNS with your domain provider:**
   - Add a **CNAME record**:
     ```
     Name: www (or your subdomain)
     Value: yourusername.github.io
     ```

3. **Enable custom domain in GitHub:**
   - Go to repository **Settings** → **Pages**
   - Enter your subdomain in the "Custom domain" field
   - Check "Enforce HTTPS" (recommended)

### Recommended: Both Apex and WWW

For the best user experience, configure both your apex domain and www subdomain:

1. Set up A records for apex domain (as shown above)
2. Set up CNAME record for www subdomain (as shown above)
3. Use your apex domain (`example.com`) in the CNAME file
4. GitHub will automatically redirect www to your apex domain

## Customization

### Personalizing Your Site

Edit `index.html` to customize:

1. **Header Section:**
   - Update "Your Name" with your actual name
   - Modify the tagline to describe yourself

2. **About Section:**
   - Write your own bio and introduction

3. **Social Links:**
   - Replace placeholder URLs with your actual social media profiles:
     - GitHub: `https://github.com/yourusername`
     - LinkedIn: `https://linkedin.com/in/yourusername`
     - Twitter: `https://twitter.com/yourusername`
     - Email: `mailto:your.email@example.com`

4. **Projects Section:**
   - Update project titles, descriptions, and links
   - Add or remove project cards as needed

5. **Footer:**
   - Update the copyright year and name

### Styling Changes

Edit `style.css` to customize:

- **Colors:** Modify the gradient colors in the `body` and `.name` selectors
- **Fonts:** Change the `font-family` in the body selector
- **Spacing:** Adjust padding and margin values
- **Animations:** Modify transition durations and effects

## File Structure

```
├── index.html    # Main HTML file
├── style.css     # Stylesheet
├── CNAME         # Custom domain configuration
├── README.md     # This file
└── LICENSE       # MIT License
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing

Feel free to submit issues and pull requests for improvements!

---

Made with ❤️ for the open source community
