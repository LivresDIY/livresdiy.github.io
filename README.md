# Company Website

A Jekyll-based website for our company, designed to be deployed on GitHub Pages.

## Quick Start

### Prerequisites

- Ruby (version 2.7 or higher)
- Bundler gem
- Git

### Local Development

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/livres-website.git
   cd livres-website
   ```

2. **Install dependencies:**
   ```bash
   bundle install
   ```

3. **Run the site locally:**
   ```bash
   bundle exec jekyll serve
   ```

4. **View the site:**
   Open your browser and go to `http://localhost:4000`

### Making Changes

- **Edit content:** Modify the Markdown files (`.md`) in the root directory and subdirectories
- **Update site settings:** Edit `_config.yml`
- **Customize styling:** Modify files in the `_sass` directory (if created)
- **Add new pages:** Create new Markdown files with appropriate front matter

## Deployment to GitHub Pages

This site uses GitHub Pages' **automatic Jekyll building** - no custom workflow needed!

### Setup Steps:

1. **Create a GitHub repository** named `livres-website` (or your preferred name)

2. **Update configuration:**
   - Edit `_config.yml` and update the following fields:
     - `title`: Your company name
     - `email`: Your contact email
     - `description`: Your company description
     - `url`: Your GitHub Pages URL (e.g., `https://yourusername.github.io`)
     - `github_username`: Your GitHub username
     - `twitter_username`: Your Twitter handle (optional)
     - `repository`: Your repository name (e.g., `yourusername/livres-website`)

3. **Push to GitHub:**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/yourusername/livres-website.git
   git push -u origin main
   ```

4. **Enable GitHub Pages:**
   - Go to your repository settings
   - Navigate to "Pages" section
   - Under "Source", select "Deploy from a branch"
   - Choose "main" branch and "/ (root)" folder
   - GitHub will automatically build and deploy your Jekyll site!

5. **Access your site:**
   Your site will be available at `https://yourusername.github.io/livres-website/`

### Custom Domain (Optional)

To use a custom domain:

1. Add a `CNAME` file to the root directory with your domain name
2. Configure your domain's DNS settings to point to GitHub Pages
3. Update the `url` field in `_config.yml` to your custom domain

## File Structure

```
├── _config.yml          # Site configuration
├── _layouts/            # Page layouts
│   └── default.html     # Default layout template
├── _includes/           # Reusable components
│   ├── head.html        # HTML head section
│   ├── header.html      # Site header
│   ├── footer.html      # Site footer
│   └── social.html      # Social media links
├── assets/
│   └── main.scss        # Custom styling
├── index.md             # Home page
├── about.md             # About page
├── contact.md           # Contact page
├── Gemfile              # Ruby dependencies
├── .gitignore           # Git ignore rules
└── README.md            # This file
```

## Customization

### Adding New Pages

Create a new Markdown file with front matter:

```markdown
---
layout: default
title: Page Title
permalink: /page-url/
---

# Page Content

Your page content goes here.
```

### Styling

This site uses the Minima theme. To customize:

1. Create a `_sass` directory
2. Add custom SCSS files
3. Import them in `assets/main.scss`

### Adding Blog Posts

1. Create a `_posts` directory
2. Add posts with filename format: `YYYY-MM-DD-title.md`
3. Include proper front matter with `layout: post`

## Support

For Jekyll documentation, visit [https://jekyllrb.com/](https://jekyllrb.com/)
For GitHub Pages documentation, visit [https://pages.github.com/](https://pages.github.com/)

## License

This project is open source and available under the [MIT License](LICENSE).
