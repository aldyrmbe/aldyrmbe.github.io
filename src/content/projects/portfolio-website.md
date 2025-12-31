---
title: "Personal Portfolio & Blog"
description: "A modern, performant portfolio website built with Astro, featuring a dark terminal-inspired design, blog functionality, and blazing-fast performance."
technologies: ["Astro", "TypeScript", "Tailwind CSS", "Markdown"]
github: "https://github.com/aldyrambe/portfolio"
live: "https://aldyrambe.dev"
featured: true
order: 1
---

# Personal Portfolio & Blog

This is the very website you're browsing right now! A carefully crafted portfolio and blog built from the ground up.

## The Challenge

I wanted to create a portfolio that:
- Reflects my personality and technical style
- Loads incredibly fast
- Makes writing and publishing content effortless
- Stands out from typical portfolio templates

## The Solution

### Technology Stack

I chose **Astro** as the foundation for its content-first approach and excellent performance characteristics. Combined with **Tailwind CSS** for styling and **TypeScript** for type safety, it's a powerful stack.

### Design Philosophy

The "Terminal Noir" aesthetic draws inspiration from:
- Code editors and terminal interfaces
- Dark mode aesthetics popular among developers
- Minimalist design with purposeful accents

### Key Features

- **Dark/Light Mode**: System-aware with manual toggle
- **Markdown Blog**: Write posts in Markdown with syntax highlighting
- **Responsive Design**: Looks great on all devices
- **SEO Optimized**: Built-in sitemap and meta tags
- **Zero JavaScript by Default**: Only hydrates when necessary

## Technical Highlights

```typescript
// Content Collections with type-safe schemas
const blog = defineCollection({
  schema: z.object({
    title: z.string(),
    description: z.string(),
    pubDate: z.coerce.date(),
    tags: z.array(z.string()),
  }),
});
```

## Lessons Learned

Building this portfolio taught me valuable lessons about:
- The importance of performance budgets
- How to create effective design systems
- Writing maintainable CSS with Tailwind

## What's Next

I plan to continue iterating on this portfolio, adding features like:
- Search functionality
- Comments system
- RSS feed
- More interactive elements

