# BAMM Digital Website

This is the static website for BAMM Digital, a digital transformation and process improvement consultancy for SMEs.

## GitHub Pages Setup Instructions

Follow these steps to host this website on GitHub Pages:

### 1. Create a GitHub Repository
- Go to [GitHub](https://github.com) and create a new repository named `bammdigital.github.io` (replace `bammdigital` with your GitHub username)
- Or create a repository with any name and enable GitHub Pages in the repository settings

### 2. Clone the Repository
```bash
git clone https://github.com/YOUR_USERNAME/bammdigital.github.io.git
cd bammdigital.github.io
```

### 3. Add the Website Files
Copy all files from this directory into your local repository:
- `index.html`
- `404.html`
- `.nojekyll`
- `assets/` directory

### 4. Commit and Push
```bash
git add .
git commit -m "Initial website deployment"
git push origin main
```

### 5. Enable GitHub Pages
- Go to your repository settings
- Scroll to "GitHub Pages" section
- Select `main` branch as the source
- Your site will be published at `https://YOUR_USERNAME.github.io`

## File Structure

```
├── index.html              # Main HTML file (all pages are routed through this)
├── 404.html               # Custom 404 page (same as index.html for SPA routing)
├── .nojekyll              # Tells GitHub Pages to skip Jekyll processing
├── assets/
│   ├── index-DIpjwk0Y.js  # Compiled JavaScript
│   └── index-Dfloycxw.css # Compiled CSS
└── __manus__/             # Debug utilities (can be removed)
```

## Custom Domain Setup

To use a custom domain (e.g., `www.bammdigital.co.uk`):

1. Add a `CNAME` file to the root directory with your domain name
2. Configure your domain registrar's DNS settings to point to GitHub Pages
3. Follow GitHub's [custom domain setup guide](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site)

## Updating the Website

To update the website content:

1. Modify the source files in the original React project
2. Run `pnpm build` to generate new static files
3. Copy the new files to your GitHub Pages repository
4. Commit and push the changes

## Support

For more information about GitHub Pages, visit: https://pages.github.com/
