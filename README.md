# Jennifer Andréoli-Fang's Personal Website

This is a personal website built with Jekyll, designed to be hosted on GitHub Pages. The site features a clean, modern design and is fully responsive. The site is accessible at both `nextjen.ai` (custom domain) and `nextjen-ai.github.io` (GitHub Pages domain).

## Features

- Modern, responsive design with clean typography
- Hero image with optimized sizing for desktop and mobile
- Professional navigation with mobile menu
- Social media integration (LinkedIn, Email, Instagram)
- Multiple content pages (Bio, CV, Projects, Publications)
- Hidden wedding page with custom pink theme (`/chapman-fang-wedding.html`)
- SEO optimized with proper meta tags
- Fast loading times with optimized assets
- Clean footer design inspired by modern personal sites
- Custom domain support via CNAME

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
├── CNAME                        # Custom domain configuration
├── _data/
│   └── site.yml                 # Site data (social links, navigation)
├── _includes/
│   ├── cv-content.html          # CV page content
│   ├── home-content.html        # Home page hero and content
│   ├── projects-content.html    # Projects page content
│   ├── paintings-content.html   # Paintings gallery content
│   └── publications-content.html # Publications page content
├── _layouts/
│   ├── bio_section.html         # Bio section layout
│   ├── default.html             # Main site layout
│   └── wedding.html             # Wedding page layout
├── _site/                       # Generated site (gitignored)
├── assets/
│   ├── css/
│   │   ├── main.css             # Main stylesheet
│   │   └── wedding-theme.css    # Wedding page pink theme
│   └── images/
│       ├── placeholder.md       # Image placeholder
│       ├── profile.jpg          # Hero profile image
│       ├── Santorini.jpg        # Wedding hero image
│       ├── Boulder.jpg          # Boulder background image
│       └── paintings/           # Painting images
│           ├── acropolis.jpg    # Painting: Acropolis
│           ├── flatirons.jpg    # Painting: Flatirons
│           ├── bhutan.jpg       # Painting: Bhutan
│           ├── lake.jpg         # Painting: Lake (portrait)
│           └── barn.jpg         # Painting: Barn
├── favicon/
│   ├── favicon.svg              # Main favicon (SVG format)
│   ├── generate-favicons.html   # Tool to generate PNG/ICO versions
│   └── README.md                # Detailed favicon documentation
├── bio.md                       # About page
├── cv.md                        # CV page
├── chapman-fang-wedding.html    # Hidden wedding page
├── index.html                   # Home page
├── projects.md                  # Projects page
├── publications.md              # Publications page
├── life-list.md                 # Personal bucket list (hidden from navigation)
├── paintings.md                 # Paintings gallery page
├── Gemfile                      # Ruby dependencies
├── Gemfile.lock                 # Locked dependencies
├── .cursor/
│   └── rules/                   # Cursor IDE rules for development
│       ├── jekyll-website.mdc   # Main project guidelines
│       ├── css-styling.mdc      # CSS and styling guidelines
│       ├── content-management.mdc # Content and SEO guidelines
│       ├── deployment.mdc       # GitHub Pages deployment guidelines
│       ├── accessibility.mdc    # WCAG AA accessibility guidelines
│       ├── seo-optimization.mdc # SEO and performance guidelines
│       └── git-commit.mdc       # Git commit and documentation guidelines
└── README.md                    # This file
```

## Content Management

### Pages
- **Home** (`index.html`): Hero section with introduction and highlights
- **Bio** (`bio.md`): About page with professional background
- **CV** (`cv.md`): Detailed resume and experience
- **Projects** (`projects.md`): Portfolio of work and projects
- **Publications** (`publications.md`): Academic papers and presentations
- **Life List** (`life-list.md`): Personal bucket list of goals and achievements (hidden from navigation)
- **Paintings** (`paintings.md`): Gallery of original oil paintings, with landscape and portrait images, and availability labels
- **Wedding** (`chapman-fang-wedding.html`): Hidden wedding page with custom pink theme

### Styling
- **Main CSS** (`assets/css/main.css`): Global styles and responsive design
- **Wedding Theme CSS** (`assets/css/wedding-theme.css`): Pink theme for wedding page
- **Page-specific styles**: Inline styles in each page for custom layouts

### Configuration
- **Site Data** (`_data/site.yml`): Social links, navigation, and site metadata
- **Jekyll Config** (`_config.yml`): Site-wide settings and plugins
- **Custom Domain** (`CNAME`): Custom domain configuration for nextjen.ai

## Development Tools

### Cursor IDE Rules
This project includes comprehensive Cursor IDE rules (`.cursor/rules/`) to ensure consistent development practices:

- **jekyll-website.mdc**: Main project guidelines and file structure
- **css-styling.mdc**: Responsive design and accessibility standards
- **content-management.mdc**: Content workflow and SEO optimization
- **deployment.mdc**: GitHub Pages deployment and custom domain setup
- **accessibility.mdc**: WCAG AA compliance guidelines
- **seo-optimization.mdc**: Meta tags, structured data, and performance
- **git-commit.mdc**: Conventional commit format and documentation updates

These rules help maintain code quality, accessibility standards, and consistent development practices across the project.

## Customization

- Edit `_data/site.yml` to update social links and navigation
- Modify `assets/css/main.css` for global styling changes
- Update page content in the respective `.md` and `.html` files
- Add new pages by creating new files with appropriate front matter
- Customize hero image by replacing `assets/images/profile.jpg`

## Recent Updates

### Footer Styling (August 2025)
- Updated footer background to match main content area (white background)
- Changed footer text and social icons to primary color for better contrast
- Improved visual consistency across the site with seamless background flow

### Development Tools (July 2025)
- Added comprehensive Cursor IDE rules for consistent development practices
- Implemented conventional commit format with automatic README update reminders
- Added accessibility guidelines for WCAG AA compliance
- Included SEO optimization guidelines for better search engine visibility
- Created deployment guidelines for GitHub Pages and custom domain management
- Added content management guidelines for consistent content workflow
- Established CSS styling guidelines for responsive design and maintainability

### Life List Page (July 2025)
- Added personal bucket list page with goals and achievements
- Implemented clean checkmark style for completed items
- Created auto-numbered list for easy rearrangement
- Hidden from main navigation for privacy while remaining accessible via direct URL
- Added invitation for visitor recommendations and suggestions

### Wedding Page (July 2025)
- Added hidden wedding page with custom pink theme (`/chapman-fang-wedding.html`)
- Created dedicated wedding layout (`_layouts/wedding.html`)
- Implemented pink wedding theme CSS (`assets/css/wedding-theme.css`)
- Added wedding hero image (`assets/images/wedding.jpg`)
- Included comprehensive wedding details: locations, agenda, guest list, local recommendations
- Added Google Maps integration for all locations
- Responsive design optimized for mobile and desktop

### Domain Configuration (July 2025)
- Added custom domain support via CNAME file
- Site now accessible at both `nextjen.ai` and `nextjen-ai.github.io`
- Configured GitHub Pages for custom domain

### Favicon Implementation (July 2025)
- Added custom "nextjen" favicon with brand colors
- Implemented SVG favicon for modern browser support
- Created organized favicon folder with documentation
- Added favicon to both main site and wedding page layouts
- See `favicon/README.md` for detailed technical documentation

### Paintings Page (July 2025)
- Added a new Paintings gallery page (`/paintings/`) showcasing original oil paintings
- Features a responsive grid with both landscape and portrait images
- Each painting displays title, medium, and availability (e.g., "SOLD", "available")
- Lake painting is displayed in portrait orientation, others in landscape
- Navigation menu updated to include "Paintings" as the rightmost option

### General Updates
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