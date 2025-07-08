# Jennifer Andréoli-Fang's Personal Website

This is a personal website built with Jekyll, designed to be hosted on GitHub Pages. The site features a clean, modern design and is fully responsive.

## Features

- Modern, responsive design with clean typography
- Hero image with optimized sizing for desktop and mobile
- Professional navigation with mobile menu
- Social media integration (LinkedIn, Email, Instagram)
- Multiple content pages (Bio, CV, Projects, Publications)
- SEO optimized with proper meta tags
- Fast loading times with optimized assets
- Clean footer design inspired by modern personal sites

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
├── _config.yml                  # Jekyll configuration
├── _data/
│   └── site.yml                 # Site data (social links, navigation)
├── _includes/
│   ├── cv-content.html          # CV page content
│   ├── home-content.html        # Home page hero and content
│   ├── projects-content.html    # Projects page content
│   └── publications-content.html # Publications page content
├── _layouts/
│   ├── bio_section.html         # Bio section layout
│   └── default.html             # Main site layout
├── _site/                       # Generated site (gitignored)
├── assets/
│   ├── css/
│   │   └── main.css             # Main stylesheet
│   └── images/
│       ├── placeholder.md       # Image placeholder
│       └── profile.jpg          # Hero profile image
├── bio.md                       # About page
├── cv.md                        # CV page
├── index.html                   # Home page
├── projects.md                  # Projects page
├── publications.md              # Publications page
├── Gemfile                      # Ruby dependencies
├── Gemfile.lock                 # Locked dependencies
└── README.md                    # This file
```

## Content Management

### Pages
- **Home** (`index.html`): Hero section with introduction and highlights
- **Bio** (`bio.md`): About page with professional background
- **CV** (`cv.md`): Detailed resume and experience
- **Projects** (`projects.md`): Portfolio of work and projects
- **Publications** (`publications.md`): Academic papers and presentations

### Styling
- **Main CSS** (`assets/css/main.css`): Global styles and responsive design
- **Page-specific styles**: Inline styles in each page for custom layouts

### Configuration
- **Site Data** (`_data/site.yml`): Social links, navigation, and site metadata
- **Jekyll Config** (`_config.yml`): Site-wide settings and plugins

## Customization

- Edit `_data/site.yml` to update social links and navigation
- Modify `assets/css/main.css` for global styling changes
- Update page content in the respective `.md` and `.html` files
- Add new pages by creating new files with appropriate front matter
- Customize hero image by replacing `assets/images/profile.jpg`

## Recent Updates

- Optimized hero image sizing (70% on desktop, 100% on mobile)
- Added social media links (LinkedIn, Email, Instagram)
- Removed copyright footer for cleaner design
- Fixed bio page spacing and layout
- Updated publications to use numbered lists
- Improved responsive design and mobile experience

## Contributing

Feel free to submit issues and enhancement requests.

## License

This project is licensed under the MIT License - see the LICENSE file for details. 