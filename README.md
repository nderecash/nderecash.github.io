# nderecash.github.io

Personal portfolio and blog for Moses Nderemani — researcher, maker, writer.

Built with Jekyll, hosted on GitHub Pages.

---

## Setup

### 1. Create the GitHub repository

1. Go to GitHub and create a new repository named **exactly** `nderecash.github.io`
2. Set it to public
3. Do **not** initialise with a README (you already have this one)

### 2. Push this code

```bash
cd nderecash.github.io
git init
git add .
git commit -m "Initial site"
git branch -M main
git remote add origin https://github.com/nderecash/nderecash.github.io.git
git push -u origin main
```

### 3. Enable GitHub Pages

In your repository settings → **Pages** → Source: **Deploy from a branch** → Branch: `main` / `/ (root)`

GitHub will build and deploy the site automatically. It usually takes 1–3 minutes. Your site will be live at **https://nderecash.github.io**.

---

## Adding blog posts

Create a new file in `_posts/` following the naming convention:

```
YYYY-MM-DD-post-title-slug.md
```

Frontmatter template:

```yaml
---
layout: post
title: "Your Post Title"
date: 2026-01-15
categories: [Research]          # Research | Making | Life | Reflection
tags: [HCI, Accessibility]
read_time: 5                    # estimated minutes
excerpt: "One sentence summary shown in listings."
---

Your post content in Markdown goes here.
```

---

## Adding photos

1. Add your images to `assets/images/photos/`
2. Create or update `_data/photos.yml`:

```yaml
- src: /assets/images/photos/tampere-winter.jpg
  alt: Frozen lake in Tampere, winter 2025
  caption: Pyynikki, January 2025

- src: /assets/images/photos/over-the-barriers.jpg
  alt: Participants at Over the Barriers tournament, Nokia Arena
  caption: Over the Barriers, Nokia Arena, April 2025
```

---

## Updating the CV

Edit `cv.md` directly — it's plain Markdown with some HTML for the two-column layout. No special build step needed.

---

## Local development (optional)

If you want to preview locally before pushing:

```bash
# Install Ruby and Bundler first (https://jekyllrb.com/docs/installation/)
bundle install
bundle exec jekyll serve
# Open http://localhost:4000
```

---

## Customisation

| What | Where |
|---|---|
| Colours, fonts, spacing | `_sass/_variables.scss` |
| Header & footer content | `_includes/header.html`, `_includes/footer.html` |
| Site title, social links | `_config.yml` |
| Home page layout | `index.html` |
