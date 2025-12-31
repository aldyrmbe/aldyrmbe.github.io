# Aldy Rambe - Personal Portfolio & Blog

A modern, performant portfolio website and blog built with Astro, featuring a dark terminal-inspired "Terminal Noir" design aesthetic.

## Features

- **Dark/Light Mode** - System-aware theme with manual toggle and localStorage persistence
- **Blog with Markdown** - Write posts in Markdown with syntax highlighting and frontmatter
- **Project Showcase** - Filterable project gallery with detailed case study pages
- **Responsive Design** - Looks great on all devices
- **SEO Optimized** - Built-in sitemap, meta tags, and Open Graph support
- **RSS Feed** - Automatic RSS feed generation for blog subscribers
- **Performance First** - Zero JavaScript by default, only hydrates when necessary

## Tech Stack

- **[Astro](https://astro.build/)** - Static site framework
- **[Tailwind CSS](https://tailwindcss.com/)** - Utility-first CSS
- **[TypeScript](https://www.typescriptlang.org/)** - Type safety
- **[Shiki](https://shiki.style/)** - Syntax highlighting

## Getting Started

### Prerequisites

- Node.js 18+ 
- npm or pnpm

### Installation

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build

# Preview production build
npm run preview
```

## Project Structure

```
├── public/              # Static assets
│   ├── favicon.svg
│   └── images/
├── src/
│   ├── components/      # Reusable Astro components
│   │   ├── Header.astro
│   │   ├── Footer.astro
│   │   ├── ThemeToggle.astro
│   │   ├── Terminal.astro
│   │   ├── ProjectCard.astro
│   │   └── BlogCard.astro
│   ├── content/         # Markdown content
│   │   ├── blog/        # Blog posts
│   │   └── projects/    # Project case studies
│   ├── layouts/         # Page layouts
│   │   ├── BaseLayout.astro
│   │   ├── BlogLayout.astro
│   │   └── ProjectLayout.astro
│   ├── pages/           # Routes
│   │   ├── index.astro
│   │   ├── about.astro
│   │   ├── blog/
│   │   ├── projects/
│   │   └── rss.xml.ts
│   └── styles/
│       └── global.css   # Global styles and theme
├── astro.config.mjs     # Astro configuration
├── content.config.ts    # Content collection schemas
└── tailwind.config.mjs  # Tailwind configuration
```

## Content Management

### Adding a Blog Post

Create a new `.md` file in `src/content/blog/`:

```markdown
---
title: "Your Post Title"
description: "A brief description of your post"
pubDate: 2024-01-15
tags: ["javascript", "tutorial"]
category: "Technology"
draft: false
---

Your content here...
```

### Adding a Project

Create a new `.md` file in `src/content/projects/`:

```markdown
---
title: "Project Name"
description: "Brief project description"
technologies: ["React", "Node.js", "PostgreSQL"]
github: "https://github.com/username/repo"
live: "https://project.example.com"
featured: true
order: 1
---

Detailed project writeup...
```

## Customization

### Colors

Edit the theme variables in `src/styles/global.css`:

```css
@theme {
  --color-accent-cyan: #22d3ee;
  --color-accent-emerald: #10b981;
  /* ... other colors */
}
```

### Site Metadata

Update `astro.config.mjs` with your site URL:

```js
export default defineConfig({
  site: 'https://your-domain.com',
  // ...
});
```

## Deployment

This site can be deployed to any static hosting platform:

- **[Vercel](https://vercel.com)** - Zero-config deployment
- **[Netlify](https://netlify.com)** - Simple git-based deployment
- **[Cloudflare Pages](https://pages.cloudflare.com)** - Edge-first hosting

```bash
# Build the site
npm run build

# The output will be in the ./dist directory
```

## License

MIT License - feel free to use this as a template for your own portfolio!

---

Built with ❤️ using [Astro](https://astro.build)
