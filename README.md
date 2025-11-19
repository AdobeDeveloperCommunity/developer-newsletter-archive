# Adobe Developer Newsletter Archive

A public archive of the Adobe Creative Cloud Developer newsletter, accessible via GitHub Pages.

## 🌐 View the Archive

Visit the live archive at: `https://[your-org].github.io/developer-newsletter-archive/`

The archive displays thumbnails of all newsletter editions, with each thumbnail linking to the full newsletter HTML.

## 📁 Repository Structure

```
developer-newsletter-archive/
├── index.html                    # Main gallery page (GitHub Pages home)
├── newsletters/                  # Newsletter HTML files
│   ├── 2024-01-newsletter.html
│   ├── 2024-02-newsletter.html
│   └── 2024-03-newsletter.html
└── .github/
    └── workflows/
        └── pages.yml             # GitHub Pages deployment workflow
```

## 📧 Adding New Newsletters

To add a new newsletter to the archive:

1. Create your newsletter as an HTML file
2. Save it in the `newsletters/` directory with the naming convention: `YYYY-MM-newsletter.html`
   - Example: `2024-04-newsletter.html`
3. Add the filename to the `newsletters` array in `index.html` (around line 257)
4. Commit and push your changes to the `main` branch
5. GitHub Actions will automatically deploy the updated site

## 🎨 Features

- **Thumbnail Previews**: Each newsletter is displayed as a thumbnail using an iframe preview
- **Responsive Design**: Grid layout adapts to different screen sizes
- **Hover Effects**: Interactive hover states show "View Newsletter" overlay
- **Auto-sorting**: Newsletters are automatically sorted by date (newest first)
- **Direct Links**: Click any thumbnail to view the full newsletter in a new tab

## 🚀 GitHub Pages Setup

The repository includes a GitHub Actions workflow (`.github/workflows/pages.yml`) that automatically deploys to GitHub Pages when changes are pushed to the main branch.

To enable GitHub Pages:
1. Go to your repository Settings
2. Navigate to "Pages" section
3. Under "Source", select "GitHub Actions"
4. The workflow will run automatically on the next push to main

## 🛠️ Development

To test locally:
1. Clone the repository
2. Open `index.html` in a web browser
3. Or use a local server: `python -m http.server 8000`
4. Navigate to `http://localhost:8000`

## 📝 Newsletter Format

Newsletters can use any HTML/CSS format. The example newsletters included demonstrate:
- Responsive design
- Clean typography
- Brand-appropriate color schemes
- Section-based content organization

## 📄 License

This archive is maintained by the Adobe Developer Community.
