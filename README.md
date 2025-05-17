# Solobooks Landing Page

This is the landing page for Solobooks, built with Jekyll and TailwindCSS.

## Prerequisites

Before you begin, ensure you have the following installed:

- Ruby (version 2.7.0 or higher)
- Node.js (version 14.0.0 or higher)
- Bundler (for Ruby gems)
- npm (comes with Node.js)

## Setup

1. Clone the repository:

```bash
git clone git@github.com:oluosiname/solobooks-landing-page.git
cd solobooks-landing
```

2. Install Ruby dependencies:

```bash
bundle install
```

3. Install Node.js dependencies:

```bash
npm install
```

## Development

To run the site locally:

1. Start the Jekyll development server:

```bash
bundle exec jekyll serve
```

By default, the site will be available at `http://localhost:4000`.

To use a different port (e.g., port 3000):

```bash
bundle exec jekyll serve --port 3000
```

The site will automatically reload if you make changes to the source files.

### Project Structure

- `_includes/` - Reusable components and partial templates
- `_layouts/` - Page layout templates
- `_posts/` - Blog posts (if any)
- `assets/` - Static assets (images, CSS, JS)
- `_data/` - Site data files
- `src/` - Source files
- `_config.yml` - Jekyll configuration
- `Gemfile` - Ruby dependencies
- `package.json` - Node.js dependencies

## Deployment

This site is deployed on Vercel. Here's how to deploy:

### Deploying to Vercel

1. Install the Vercel CLI:

```bash
npm install -g vercel
```

2. Login to Vercel:

```bash
vercel login
```

3. Deploy:

```bash
vercel
```

For production deployment:

```bash
vercel --prod
```

### Environment Variables

If needed, set up environment variables in your Vercel project settings.

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the terms specified in the LICENSE file.
