# GitHub Pages Setup Guide for Your Academic Website

Your personal academic website is now ready to be deployed on GitHub Pages. Follow these steps to get it live:

## Prerequisites

- A GitHub account (free)
- Git installed on your computer
- Basic terminal/command line knowledge

## Step 1: Create a GitHub Repository

1. Go to [github.com](https://github.com) and sign in to your account
2. Click the **+** icon in the top right and select **New repository**
3. Name your repository: **`naveenjesubalan.github.io`** (replace with your GitHub username)
4. Make sure it's **Public**
5. Click **Create repository**

## Step 2: Initialize Git and Push Code

Open Terminal and navigate to your website folder:

```bash
cd /Users/naveenj/Documents/NJ/My_website
```

Initialize git and push your code:

```bash
git init
git add .
git commit -m "Initial commit: Academic website"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_USERNAME.github.io.git
git push -u origin main
```

Replace `YOUR_USERNAME` with your actual GitHub username.

## Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings**
3. Scroll to **Pages** section (left sidebar)
4. Under "Source", select **Deploy from a branch**
5. Select **main** branch and **/ (root)** folder
6. Click **Save**

Your site will be live at: `https://YOUR_USERNAME.github.io`

## Step 4: Build Locally (Optional)

To preview changes before pushing:

```bash
# Install dependencies
bundle install

# Build and serve locally
bundle exec jekyll serve
```

Visit `http://localhost:4000` to see your site.

## Customization Guide

### Update Your Information

Edit the following files:

- **[_config.yml](_config.yml)** - Site title, email, social links
- **[index.md](index.md)** - Homepage content
- **[about.md](about.md)** - About page
- **[publications.md](publications.md)** - Publication list
- **[cv.md](cv.md)** - CV page

### Customize Colors

Edit **[assets/css/style.css](assets/css/style.css)** and modify the `:root` CSS variables:

```css
:root {
  --primary-color: #2c3e50;      /* Main text/headings */
  --accent-color: #3498db;       /* Links/highlights */
  --light-bg: #ecf0f1;           /* Light backgrounds */
}
```

### Add More Pages

1. Create a new `.md` file in the root directory
2. Add front matter at the top:

```yaml
---
layout: default
title: Page Title
---

# Page Title

Your content here...
```

3. Add navigation link in **[_includes/nav.html](_includes/nav.html)**

## File Structure

```
My_website/
├── index.md                 # Homepage
├── about.md                # About page
├── publications.md         # Publications list
├── cv.md                   # CV page
├── Publications.csv        # Your publication data
├── _config.yml             # Jekyll configuration
├── Gemfile                 # Ruby dependencies
├── .gitignore              # Files to ignore in git
├── _layouts/
│   └── default.html        # Main layout template
├── _includes/
│   ├── nav.html           # Navigation bar
│   └── footer.html        # Footer
└── assets/
    └── css/
        └── style.css      # Website styling
```

## Next Steps

1. **Add a Profile Photo** (Optional):
   - Place an image in `assets/images/profile.jpg`
   - Update `index.md` to include: `![Profile](/assets/images/profile.jpg)`

2. **Add a Blog** (Optional):
   - Create `_posts/` folder
   - Add posts as `YYYY-MM-DD-title.md`

3. **Connect Custom Domain** (Optional):
   - Go to Settings > Pages
   - Add your custom domain under "Custom domain"
   - Update DNS settings at your domain registrar

4. **Add Google Analytics** (Optional):
   - Add your Google Analytics ID to `_config.yml`

## Troubleshooting

### Site not showing up?
- Wait 5-10 minutes after pushing
- Check Settings > Pages for any error messages
- Ensure repository name is exactly `USERNAME.github.io`

### Changes not appearing?
- Hard refresh browser (Cmd+Shift+R on Mac)
- Check if build succeeded in repository Settings > Pages

### Build failed?
- Check the error email from GitHub
- Ensure `Gemfile` is correct
- Test locally with `bundle exec jekyll serve`

## Support & Resources

- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Markdown Guide](https://www.markdownguide.org/)

---

**Your website is now ready! Start with the customization steps above to personalize it further.**
