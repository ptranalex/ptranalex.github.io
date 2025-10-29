# 🧠 Alex Tran — Blog & Portfolio

A personal blog and portfolio built with **Jekyll** and the **Minimal Mistakes** theme, hosted on **GitHub Pages**.  
This site is my digital notebook — where I write about **engineering, AI, automation, and leadership**, and showcase the systems and experiments I build.

## 🚀 Quick Start

### Local Development

1. **Install Ruby and Bundler** (if not already installed):

   ```bash
   # On macOS with Homebrew
   brew install ruby
   gem install bundler
   ```

2. **Install dependencies**:

   ```bash
   bundle install
   ```

3. **Run the site locally**:

   ```bash
   bundle exec jekyll serve
   ```

4. **View the site**: Open your browser to `http://localhost:4000`

### Making Changes

The site will automatically rebuild when you make changes to files. Just refresh your browser to see the updates.

## 📁 Site Structure

```
.
├── _config.yml          # Site configuration
├── _posts/              # Blog posts (YYYY-MM-DD-title.md format)
├── _pages/              # Static pages (about, blog archive, etc.)
├── _portfolio/          # Portfolio items
├── assets/              # Images, CSS, JavaScript
│   └── images/         # Site images
├── index.md            # Homepage
└── Gemfile             # Ruby dependencies
```

## ✍️ Creating Content

### Writing a Blog Post

Create a new file in `_posts/` with the format: `YYYY-MM-DD-title.md`

```markdown
---
title: "Your Post Title"
date: 2025-10-29
categories:
  - category1
tags:
  - tag1
  - tag2
excerpt: "A brief description of your post"
---

Your content here...
```

### Adding a Portfolio Item

Create a new file in `_portfolio/` with a descriptive name:

```markdown
---
title: "Project Name"
excerpt: "Brief project description"
header:
  teaser: /assets/images/project-teaser.jpg
sidebar:
  - title: "Role"
    text: "Your Role"
  - title: "Technologies"
    text: "Tech stack used"
---

Your project details here...
```

## 🎨 Customization

### Site Settings

Edit `_config.yml` to customize:

- Site title, description, and URL
- Author information and social links
- Theme skin/appearance
- Navigation menu

### Theme Customization

The Minimal Mistakes theme offers several skins. Change the skin in `_config.yml`:

```yaml
minimal_mistakes_skin: "default" # "air", "aqua", "contrast", "dark", "dirt", "neon", "mint", "plum", "sunrise"
```

### Adding Images

Place images in `assets/images/` and reference them in your posts:

```markdown
![Alt text](/assets/images/your-image.jpg)
```

## 🚢 Deployment

### GitHub Pages

This site is configured to work with GitHub Pages out of the box:

1. **Commit your changes**:

   ```bash
   git add .
   git commit -m "Your commit message"
   ```

2. **Push to GitHub**:

   ```bash
   git push origin main
   ```

3. **GitHub Pages will automatically build and deploy** your site to `https://ptranalex.github.io`

### Build Time

It may take a few minutes for changes to appear on your live site after pushing.

## 📚 Resources

- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [Minimal Mistakes Documentation](https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Markdown Guide](https://www.markdownguide.org/)

## 🛠️ Troubleshooting

### Site not building?

1. Check the Actions tab in your GitHub repository for build errors
2. Ensure your `_config.yml` is valid YAML
3. Make sure all required plugins are listed in the `Gemfile`

### Local development issues?

1. Run `bundle update` to update dependencies
2. Clear the Jekyll cache: `bundle exec jekyll clean`
3. Restart the server

## 📝 Next Steps

1. **Personalize** the `_config.yml` with your information
2. **Update** the About page with your bio
3. **Add** your own avatar image to `assets/images/avatar.jpg`
4. **Write** your first blog post
5. **Add** your portfolio projects
6. **Customize** the theme colors and styling
7. **Push** to GitHub and watch your site come to life!

## 📄 License

This project structure is free to use. The Minimal Mistakes theme is licensed under the MIT License.
