# Jennifer Andréoli-Fang's Personal Website

This is a personal website built with Jekyll, designed to be hosted on GitHub Pages. The site features a clean, modern design and is fully responsive.

Note: to test out on local server, run
```
bundle exec jekyll serve
```

## Features

- Modern, responsive design
- Clean and professional layout
- Easy to maintain and update
- SEO optimized
- Fast loading times

## Prerequisites

- Ruby (version 2.7.0 or higher)
- Bundler
- Git

## Local Development

1. Clone the repository:
```bash
git clone https://github.com/nextjen-ai/nextjen-ai.github.io.git
cd nextjen-ai.github.io
```

2. Install dependencies:
```bash
bundle install
```

3. Start the local development server:
```bash
bundle exec jekyll serve
```

4. Open your browser and visit `http://localhost:4000`

## Deployment

This site is configured to be deployed on GitHub Pages. Simply push your changes to the main branch, and GitHub Pages will automatically build and deploy your site.

## Project Structure

```
.
├── _config.yml          # Jekyll configuration
├── _layouts/           # Layout templates
├── assets/            # Static assets (CSS, images)
├── index.html         # Home page
├── bio.html          # Biography page
└── Gemfile           # Ruby dependencies
```

## Customization

- Edit `_config.yml` to update site-wide settings
- Modify CSS in `assets/css/main.css`
- Update content in the respective HTML files
- Add new pages by creating new HTML files with the appropriate front matter

## Contributing

Feel free to submit issues and enhancement requests.

## License

This project is licensed under the MIT License - see the LICENSE file for details. 