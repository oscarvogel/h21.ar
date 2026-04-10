# H21 - Eleventy Static Site Generator

A modern, fast static website built with [Eleventy (11ty)](https://www.11ty.dev/), styled with [Tailwind CSS](https://tailwindcss.com/) and processed with [PostCSS](https://postcss.org/).

## 🚀 Tech Stack

- **Eleventy (11ty)** v3.0.0 - Static site generator
- **Tailwind CSS** v4.0.14 - Utility-first CSS framework
- **PostCSS** v8.5.3 - CSS processing
- **Autoprefixer** v10.4.21 - CSS vendor prefix automation
- **Nunjucks** - Template engine

## 📁 Project Structure

```
h21/
├── src/                    # Source files
│   ├── _data/             # Global data files
│   ├── _includes/         # Reusable templates and components
│   ├── assets/            # Static assets (CSS, images, JS)
│   ├── contacto/          # Contact page content
│   ├── nosotros/          # About us page content
│   ├── vision_mision/     # Vision & Mission page content
│   ├── index.njk          # Homepage template
│   ├── robots.txt         # Robots exclusion file
│   └── sitemap.njk        # XML sitemap template
├── _site/                 # Generated output (deploy this folder)
├── .eleventy.js           # Eleventy configuration
├── tailwind.config.js     # Tailwind CSS configuration
├── postcss.config.js      # PostCSS configuration
└── package.json           # Node.js dependencies
```

## 🛠️ Installation

```bash
npm install
```

## 📦 Development

Start the development server with hot reload:

```bash
npm run dev
```

## 🏗️ Build

Generate production-ready files:

```bash
npm run build
```

The built files will be output to the `_site/` directory.

## ⚙️ Configuration

### Eleventy Features

- **Template Formats**: Nunjucks (`.njk`) and Markdown (`.md`)
- **Custom Collections**: `noticias` - Blog/news posts sorted by date
- **Custom Filters**:
  - `formatDate` - Formats dates in Spanish locale
  - `toISOString` - Converts dates to ISO format for sitemaps
- **Passthrough Copy**: Assets and robots.txt are copied directly to output
- **Deep Data Merge**: Enables recursive merging of data files

### CSS Pipeline

CSS is processed with PostCSS and Tailwind CSS for modern, optimized styles.

## 📝 Adding Content

### Blog Posts

Add markdown files to `src/blog/` with frontmatter:

```yaml
---
title: "Post Title"
date: 2026-04-10
---
```

### Pages

Create new pages by adding directories or `.njk`/`.md` files to the `src/` folder.

## 🌐 Deployment

Deploy the `_site/` folder to any static hosting service:
- Netlify
- Vercel
- GitHub Pages
- AWS S3 + CloudFront

## 📄 License

[Add your license here]

## 👥 Team

[Add team information or link to /equipo page]
