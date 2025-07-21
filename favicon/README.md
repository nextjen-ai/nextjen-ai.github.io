# Favicon Setup

This folder contains the favicon files for the nextjen-ai.github.io website.

## Files

- `favicon.svg` - The main favicon file (SVG format for scalability)
- `generate-favicons.html` - Tool to generate PNG/ICO versions if needed

## Current Implementation

The website currently uses the SVG favicon (`favicon.svg`) which provides:
- ✅ Scalable design that looks crisp at any size
- ✅ Small file size
- ✅ Modern browser support
- ✅ "nextjen" branding in your brand colors

## Design Details

- **Background**: White (#ffffff)
- **Text**: Dark blue (#2c3e50) 
- **Border**: Light gray (#e9ecef)
- **Font**: Inter (or system fallbacks)
- **Text**: "nextjen"

## Browser Support

The SVG favicon is supported by all modern browsers. For older browsers that don't support SVG favicons, you can:

1. Open `generate-favicons.html` in a browser
2. Click "Download All Favicon Files" 
3. Place the generated PNG/ICO files in the website root
4. Update the layout to include the additional favicon links

## Implementation

The favicon is implemented in `_layouts/default.html` with:
```html
<link rel="icon" type="image/svg+xml" href="{{ '/favicon/favicon.svg' | relative_url }}">
```

This provides excellent browser support while maintaining the clean, professional "nextjen" branding. 