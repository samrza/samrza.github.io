# Minimalist Blog

A clean, minimal personal blog for showcasing coding projects, writing, photography, and reading.

## Features

- **Projects** — Showcase your coding projects with links to live demos and source code
- **Blog** — Write posts; each post is a simple HTML file
- **Photography** — Photo gallery with lightbox (click to enlarge)
- **Reading** — Track books by year and what you're currently reading

## Quick start

1. Open `index.html` in a browser, or run a local server:

   ```bash
   cd /Users/sam/blog
   python3 -m http.server 8000
   ```

2. Visit [http://localhost:8000](http://localhost:8000)

## Customizing

### Add projects
Edit `projects.html` — duplicate a `project-card` block and fill in title, description, tech, and links.

### Write blog posts
1. Create a new HTML file in `posts/` (copy `posts/example-post.html` as a template)
2. Add an entry in `blog.html` — duplicate a `post-item` block

### Add photography
1. Add your images to the `images/` folder (JPG, WebP, or PNG)
2. Edit `photography.html` — update `src` and `figcaption` for each `gallery-item`

### Update reading list
Edit `reading.html` — add books to "Currently reading" or create new `year-block` sections for each year.

### Change your name
Search for "Sam" in the HTML files and replace with your name. Update the `nav-logo` and page titles.

## Structure

```
blog/
├── index.html          # Home
├── projects.html       # Coding projects
├── blog.html           # Blog post list
├── photography.html    # Photo gallery
├── reading.html        # Reading tracker
├── styles.css          # All styles
├── gallery.js          # Lightbox for photos
├── posts/              # Blog post HTML files
│   └── example-post.html
└── images/             # Your photos
    └── placeholder.svg
```

## Deploy

Upload the folder to any static host (Netlify, Vercel, GitHub Pages, etc.) — no build step required.
