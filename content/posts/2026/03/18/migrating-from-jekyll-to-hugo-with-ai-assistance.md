---
title: "Migrating from Jekyll to Hugo with AI Assistance"
date: 2026-03-18T00:00:00+05:30
description: How I used AI to migrate this blog from Jekyll to Hugo in no time.
categories:
  - hugo
  - jekyll
  - ai
---

A while back, I started this blog using Jekyll. It worked well, but over time, managing Ruby dependencies and the occasional build quirks became a bit of a hassle. When I wanted to move to Hugo, the prospect of manually converting everything felt daunting.

Enter AI. I used [OpenCode Desktop](https://opencode.ai/download) to help with the migration. Here's how it went:

**The Process**

1. First, I asked the AI to analyze the existing Jekyll structure and explain how Hugo's organization differs
2. It helped convert the front matter from YAML to TOML format
3. It generated the Hugo configuration file based on the site's needs
4. It created the necessary layout templates by understanding the existing HTML structure
5. It set up a GitHub Actions workflow to automatically build and deploy the site on every push

**What Worked Well**

- Converting post front matter was straightforward - just had to verify the dates matched
- The AI understood the minimal PaperMod theme and reproduced the key layout elements
- It caught a few broken image links I had forgotten about
- Setting up GitHub Actions for automatic deployment was quick and well-documented

**What Needed Manual Attention**

- Some Liquid template logic didn't translate directly
- Custom CSS tweaks required eyeballing to match the original look

**The Result**

The migration took a fraction of the time it would have manually. The AI didn't replace understanding the tools, but it accelerated the repetitive parts significantly.

If you're considering a similar move, I'd recommend having the documentation for both tools open. Give the AI context about what you're building, and verify everything works locally before deploying.
