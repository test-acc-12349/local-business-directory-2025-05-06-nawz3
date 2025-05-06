# Local Business Directory

> Discover the best local businesses in one place

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
- [Directory Structure](#directory-structure)
- [Customization Guide](#customization-guide)
- [Deployment](#deployment)
- [Custom Domain Setup](#custom-domain-setup)
- [Troubleshooting](#troubleshooting)
- [Support & Resources](#support--resources)

## Overview
Local Business Directory is a responsive web-based directory showcasing local businesses in a clean, three-column grid layout. The platform helps users discover and connect with local businesses through an intuitive category-based navigation system.

## Features
- Responsive 3-column grid layout
- Category-based filtering
- Search functionality
- Business detail pages
- Contact forms
- Mobile-friendly design
- SEO optimized structure
- Fast loading performance

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn
- Git

### Installation
```bash
# Clone the repository
git clone https://github.com/yourusername/local-business-directory.git

# Navigate to project directory
cd local-business-directory

# Install dependencies
npm install

# Start development server
npm run dev
```

## Directory Structure
```
local-business-directory/
├── src/
│   ├── components/
│   ├── pages/
│   ├── styles/
│   └── data/
├── public/
│   ├── images/
│   └── icons/
├── config/
└── package.json
```

## Customization Guide

### Adding Directory Items
1. Navigate to `src/data/businesses.js`
2. Add new business entry using the following format:
```javascript
{
  id: "unique-id",
  name: "Business Name",
  category: "Category",
  address: "Business Address",
  phone: "Phone Number",
  website: "Website URL",
  description: "Business Description"
}
```

### Modifying Categories
1. Open `src/data/categories.js`
2. Edit category structure:
```javascript
export const categories = [
  {
    id: "category-id",
    name: "Category Name",
    icon: "icon-name"
  }
]
```

### Updating Hero Section
1. Locate `src/components/Hero.js`
2. Modify the content:
```javascript
<div className="hero">
  <h1>Your Custom Heading</h1>
  <p>Your custom description</p>
</div>
```

### Customizing Colors
1. Edit `src/styles/variables.scss`:
```scss
$primary-color: #your-color;
$secondary-color: #your-color;
$accent-color: #your-color;
```

## Deployment

### Build for Production
```bash
npm run build
```

### Deploy to Hosting
```bash
# Example for Netlify
netlify deploy --prod
```

## Custom Domain Setup

1. Purchase domain from preferred registrar
2. Add DNS records:
```
A Record: @ -> Your-Server-IP
CNAME: www -> your-site.netlify.app
```
3. Configure hosting provider:
   - Add custom domain in settings
   - Enable HTTPS
   - Wait for DNS propagation (24-48 hours)

## Troubleshooting

### Common Issues

#### Build Failures
- Clear cache: `npm clean cache --force`
- Delete node_modules: `rm -rf node_modules`
- Reinstall dependencies: `npm install`

#### Style Issues
- Check browser compatibility
- Verify SCSS compilation
- Clear browser cache

#### Directory Items Not Showing
- Validate data format in `businesses.js`
- Check console for errors
- Verify category assignments

## Support & Resources

### Documentation
- [Component Documentation](docs/components.md)
- [API Reference](docs/api.md)
- [Style Guide](docs/style-guide.md)

### Support Channels
- GitHub Issues
- Email Support: support@localbusinessdirectory.com
- Community Forum: [Link]

### Useful Links
- [Contributing Guidelines](CONTRIBUTING.md)
- [Code of Conduct](CODE_OF_CONDUCT.md)
- [License](LICENSE.md)

---

## License
MIT © [Local Business Directory]