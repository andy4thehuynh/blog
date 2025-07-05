+++
title = "How I Built My Personal Website with Hugo, GitHub Pages, and a Custom Domain"
date = "2025-07-05T13:58:33-06:00"
#dateFormat = "2006-01-02" # This value can be configured for per-post date formatting
author = ""
authorTwitter = "" #do not include @
cover = ""
tags = ["go", "github"]
keywords = ["", ""]
description = ""
showFullContent = false
readingTime = false
hideComments = false
+++

After some research and trial-and-error, I successfully built and deployed my personal website using the [Hugo static site generator](https://gohugo.io/), a minimalist theme called [Terminal](https://github.com/panr/hugo-theme-terminal), GitHub Pages for hosting, and my own domain from Porkbun. Here's how I did it:

### Step 1: I Installed Hugo

I installed Hugo on my local machine using Homebrew (macOS) or apt (Linux). It was easy to verify with `hugo version`.

### Step 2: I Created a New Site

I ran `hugo new site myblog` to scaffold a new site, then added the Terminal theme as a submodule.

### Step 3: I Customized the Config

The `config.toml` file controls everything from the site title to the menu structure. I added my own values and set the theme.

### Step 4: I Wrote My First Post

Using `hugo new posts/first-post.md`, I created this post and removed the `draft: true` line to make it live.

### Step 5: I Hosted It on GitHub Pages

I built the site with `hugo` and pushed the `public/` folder to a `gh-pages` branch. Then I enabled GitHub Pages in my repo settings.

### Step 6: I Connected My Porkbun Domain

After updating the DNS records at Porkbun and adding a `CNAME` file, my site was available at my own custom URL.

---

🎉 I'm officially online! This is just the beginning. Stay tuned for more posts on design, dev, and everything in between.
