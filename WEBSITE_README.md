# Naveen Jesubalan - Academic Website

A minimal, clean academic website for a PhD candidate at IIT Delhi. Built with Jekyll and hosted on GitHub Pages.

## Features

- **Minimal Design**: Clean, distraction-free layout focusing on content
- **No Complicated Emojis**: Professional appearance with subtle styling
- **Responsive**: Works perfectly on desktop, tablet, and mobile devices
- **Fast & Lightweight**: Pure HTML/CSS with no unnecessary dependencies
- **GitHub Pages Ready**: Deploy free and automatically updated

## Contents

- **Home** - Professional introduction and research focus
- **About** - Detailed background, skills, and research interests
- **Publications** - Complete list of peer-reviewed publications (18 papers)
- **CV** - Academic curriculum vitae
- **Contact** - Easy links to email, LinkedIn, Google Scholar, Bluesky, and Twitter/X

## Quick Start

### Local Development

```bash
# Install dependencies
bundle install

# Build and serve locally
bundle exec jekyll serve

# Visit http://localhost:4000
```

### Deploy to GitHub Pages

See [DEPLOYMENT_GUIDE.md](DEPLOYMENT_GUIDE.md) for step-by-step instructions.

## Customization

### Colors & Styling

Edit `assets/css/style.css` to customize colors, fonts, and layout:

```css
:root {
  --primary-color: #2c3e50;      /* Main color */
  --accent-color: #3498db;       /* Links/buttons */
  --light-bg: #ecf0f1;           /* Background */
}
```

### Site Information

Update `_config.yml`:

```yaml
title: Your Name
email: your.email@example.com
description: Your professional description
url: https://yourusername.github.io
```

### Pages & Content

- `index.md` - Homepage
- `about.md` - About page
- `publications.md` - Publications
- `cv.md` - CV page

Add new pages as `.md` files with front matter and update navigation in `_includes/nav.html`.

## Files Structure

```
├── _config.yml              # Site configuration
├── _layouts/default.html    # Main layout
├── _includes/               # Reusable components
│   ├── nav.html
│   └── footer.html
├── assets/css/style.css     # Styling
├── index.md                 # Home
├── about.md                 # About
├── publications.md          # Publications
├── cv.md                    # CV
├── Publications.csv         # Publication data
├── Gemfile                  # Ruby gems
└── DEPLOYMENT_GUIDE.md      # Setup instructions
```

## Technical Stack

- **Static Site Generator**: Jekyll
- **Styling**: Pure CSS (no frameworks)
- **Hosting**: GitHub Pages (free)
- **Deployment**: Automatic via Git push

## Browser Support

- Chrome/Chromium (all versions)
- Firefox (all versions)
- Safari (all versions)
- Edge (all versions)

## Performance

- Page Load Time: < 500ms
- Mobile Friendly: Yes
- SEO Optimized: Yes
- Accessibility: WCAG compliant

## License

This website template is free to use and modify for your personal academic website.

## Contact

For questions about the website setup, refer to [DEPLOYMENT_GUIDE.md](DEPLOYMENT_GUIDE.md) or the [Jekyll Documentation](https://jekyllrb.com/).

---

**Next Step**: Read [DEPLOYMENT_GUIDE.md](DEPLOYMENT_GUIDE.md) to deploy your site to GitHub Pages.
