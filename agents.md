# Project Documentation for AI Agents

## Project Overview

This is a personal blog named "Logging the Quirks" - a place for documenting unusual discoveries on random walks. Originally built with Jekyll, now using Hugo for static site generation.

## Tech Stack

- **Static Site Generator**: Hugo
- **Hosting**: GitHub Pages
- **Theme**: Custom minimal theme (PaperMod compatible)

## Project Structure

```
.
├── archetypes/       # Content templates
├── assets/          # Hugo assets (SCSS, etc.)
├── content/         # Blog posts and pages
│   ├── posts/       # Blog posts (Hugo naming: YYYY/MM/DD/post-name.md)
│   ├── about.md     # About page
│   └── _index.md    # Home page content
├── layouts/         # Custom HTML templates
├── static/          # Static files (CSS, images, etc.)
├── hugo.toml        # Hugo configuration
└── public/         # Built site output (gitignored)
```

## Content Guidelines

### Posts
- Use Hugo's date format in front matter: `date: 2017-06-05T00:02:25+05:30`
- Front matter fields: `title`, `date`, `description`, `tags`, `categories`
- Place posts in `content/posts/` with date prefix in filename

### Front Matter Example
```yaml
---
title: "Post Title"
date: 2024-01-15T10:30:00+05:30
description: "Brief description for SEO"
tags: ["tag1", "tag2"]
categories: ["category1"]
---
```

## Commands

```bash
# Development server with drafts
hugo server -D

# Build for production
hugo

# Build with drafts
hugo -D
```

## GitHub Pages Deployment

The site is deployed to GitHub Pages. The `public/` directory is the built output that gets pushed to the `gh-pages` branch or served from the repository root.

## Notes

- This is a simple blog with minimal customization
- Theme configuration is in `hugo.toml`
- No JavaScript frameworks or complex build steps
