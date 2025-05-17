# Solobooks Landing Page Documentation

{info}
This documentation covers the setup, deployment, and maintenance of the Solobooks Landing Page project.
{info}

## Table of Contents

1. [Initial Setup](#initial-setup)
2. [Local Development](#local-development)
3. [Deployment Process](#deployment-process)
4. [Adding New Pages](#adding-new-pages)
5. [Localization Guide](#localization-guide)
6. [Troubleshooting](#troubleshooting)

## Initial Setup

### Prerequisites

Before beginning, ensure you have installed:

- Ruby (version 2.7.0 or higher)
- Node.js (version 14.0.0 or higher)
- Bundler (Ruby gem manager)
- npm (Node.js package manager)

### Installation Steps

1. Clone the repository:

```bash
git clone <your-repository-url>
cd solobooks-landing
```

2. Install dependencies:

```bash
bundle install
npm install
```

{note}
If you encounter any permission issues during Ruby gem installation, try using `sudo bundle install`
{note}

## Local Development

### Starting the Development Server

1. Run the Jekyll server:

```bash
bundle exec jekyll serve
```

2. Access the site at `http://localhost:4000`

### Custom Port Configuration

To use a different port:

```bash
bundle exec jekyll serve --port <port-number>
```

{tip}
Common alternative ports: 3000, 8080, 8000
{tip}

## Deployment Process

### First-time Vercel Setup

1. Install Vercel CLI:

```bash
npm install -g vercel
```

2. Authenticate with Vercel:

```bash
vercel login
```

3. Link your project:

```bash
vercel link
```

### Deployment Commands

- For development deployment:

```bash
vercel
```

- For production deployment:

```bash
vercel --prod
```

{warning}
Always test your changes in a development deployment before pushing to production
{warning}

## Adding New Pages

### Basic Page Structure

1. Create a new `.md` file in the root directory or appropriate subdirectory:

```markdown
---
layout: default
title: Your Page Title
permalink: /your-page-url/
---

Your content here
```

### Using Layouts

Available layouts:

- `default` - Basic page layout
- `post` - Blog post layout
- `page` - Standard page layout

### Example: Adding a Blog Post

1. Create a new file in `_posts` directory:

```
_posts/YYYY-MM-DD-post-title.md
```

2. Add front matter:

```markdown
---
layout: post
title: "Your Post Title"
date: YYYY-MM-DD HH:MM:SS +0000
categories: [category1, category2]
---
```

## Localization Guide

### Adding a New Language

1. Create a new language directory:

```bash
mkdir <language-code>
```

2. Update `_config.yml`:

```yaml
languages: ["en", "de", "<language-code>"]
```

3. Create language-specific content structure:

```
<language-code>/
├── index.md
├── about.md
└── blog/
    └── index.md
```

### Translation Process

1. Copy existing content from primary language (en):

```bash
cp -r en/* <language-code>/
```

2. Translate front matter:

```yaml
---
layout: default
title: "Translated Title"
lang: <language-code>
---
```

3. Translate content while maintaining markdown structure

{note}
Remember to translate URLs in the front matter's `permalink` field
{note}

### Language-specific Configuration

In `_config.yml`, you can set language-specific variables:

```yaml
defaults:
  - scope:
      path: ""
      lang: "<language-code>"
    values:
      description: "Language-specific description"
```

## Troubleshooting

### Common Issues

1. **Jekyll Build Errors**

   - Clear cache: `bundle exec jekyll clean`
   - Update dependencies: `bundle update`

2. **Vercel Deployment Failures**

   - Check build logs: `vercel logs`
   - Verify environment variables are set correctly

3. **Missing Content**
   - Ensure front matter is properly formatted
   - Check file permissions
   - Verify language codes in `_config.yml`

### Support Resources

- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [Vercel Documentation](https://vercel.com/docs)
- Internal team contact: [Your Team Contact]

{info}
For additional support, please contact the development team through the appropriate channels.
{info}
