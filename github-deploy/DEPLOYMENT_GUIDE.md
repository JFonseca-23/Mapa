# Website Deployment Guide - Interactive Iberian Songs Platform

## Overview
This guide provides step-by-step instructions to publish your interactive Iberian songs platform as a website using various hosting solutions.

## Pre-Deployment Checklist

### Required Files for Deployment
- `index.html` (renamed from `Wrapped - final.html`)
- `thematic_map.json`
- `spanish-mei-location-mapping.json`
- `portuguese-mei-location-mapping.json`
- `song_difficulty_analysis.json`
- `Spanish/` folder (742 MEI files)
- `Portuguese/` folder (59 MEI files)

### File Size Considerations
- Total project size: ~50-100MB
- MEI files: Text-based XML (relatively small)
- No large media files (good for hosting)

## Deployment Methods

### Method 1: GitHub Pages (Free, Recommended for Academic Projects)

#### Step 1: Prepare Repository
```bash
# Create a new repository on GitHub
# Clone it locally
git clone https://github.com/yourusername/iberian-songs-map.git
cd iberian-songs-map

# Copy your files
cp "/Users/joaofonseca/Desktop/Mapa final/Wrapped - final.html" ./index.html
cp "/Users/joaofonseca/Desktop/Mapa final/"*.json ./
cp -r "/Users/joaofonseca/Desktop/Mapa final/Spanish" ./
cp -r "/Users/joaofonseca/Desktop/Mapa final/Portuguese" ./

# Add and commit
git add .
git commit -m "Initial deployment of Iberian Songs Interactive Platform"
git push origin main
```

#### Step 2: Enable GitHub Pages
1. Go to your GitHub repository
2. Click "Settings" tab
3. Scroll to "Pages" section
4. Select "Deploy from a branch"
5. Choose "main" branch and "/ (root)" folder
6. Click "Save"

**Your site will be available at**: `https://yourusername.github.io/iberian-songs-map`

### Method 2: Netlify (Easy Drag-and-Drop)

#### Step 1: Prepare Files
1. Create a folder called `iberian-songs-website`
2. Copy all necessary files (see checklist above)
3. Rename `Wrapped - final.html` to `index.html`

#### Step 2: Deploy
1. Go to [netlify.com](https://netlify.com)
2. Sign up for free account
3. Drag your project folder to the deployment area
4. Netlify will automatically deploy your site

**Features**:
- Custom domain support
- Automatic HTTPS
- Form handling capabilities
- CDN (Content Delivery Network)

### Method 3: Vercel (Modern Deployment)

#### Step 1: Install Vercel CLI
```bash
npm install -g vercel
```

#### Step 2: Deploy
```bash
cd "/Users/joaofonseca/Desktop/Mapa final"
cp "Wrapped - final.html" index.html
vercel --prod
```

### Method 4: Traditional Web Hosting

#### Recommended Providers
1. **SiteGround** - Excellent for educational sites
2. **Bluehost** - WordPress friendly
3. **HostGator** - Budget-friendly
4. **DreamHost** - Good for non-profits

#### Steps
1. Purchase hosting plan
2. Access cPanel or hosting control panel
3. Upload files via File Manager or FTP
4. Ensure `index.html` is in the public_html folder

## Custom Domain Setup

### Purchase Domain
- **Recommended registrars**: Namecheap, Google Domains, Cloudflare
- **Suggested domains**: 
  - `iberian-songs.com`
  - `cultural-heritage-map.org`
  - `spanish-portuguese-songs.net`

### DNS Configuration
Point your domain to your hosting provider's nameservers or IP address.

## Performance Optimization

### Before Deployment
1. **Minify JSON files** (optional)
2. **Compress MEI files** using gzip
3. **Enable browser caching**

### After Deployment
1. **Test loading speed** with Google PageSpeed Insights
2. **Monitor bandwidth usage**
3. **Set up analytics** (Google Analytics)

## Security Considerations

### HTTPS Setup
- Most modern hosting providers include free SSL certificates
- Ensure all external resources use HTTPS URLs

### Content Protection
- MEI files are served as static files (consider if you need access control)
- No sensitive data is exposed in the current implementation

## Maintenance and Updates

### Adding New Songs
1. Add MEI files to appropriate folders
2. Update mapping JSON files
3. Regenerate thematic mappings if needed
4. Redeploy

### Monitoring
- Set up uptime monitoring
- Monitor site traffic and usage patterns
- Regular backups of your files

## Cost Estimates

### Free Options
- **GitHub Pages**: Free (public repository)
- **Netlify**: Free tier (100GB bandwidth/month)
- **Vercel**: Free tier (100GB bandwidth/month)

### Paid Options
- **Shared Hosting**: $5-15/month
- **Cloud Hosting**: $10-50/month
- **Custom Domain**: $10-15/year

## Technical Requirements

### Browser Compatibility
Your platform uses modern web APIs:
- **Supported browsers**: Chrome 60+, Firefox 55+, Safari 12+, Edge 79+
- **Required features**: Web Audio API, SVG support, ES6 modules

### Server Requirements
- Static file hosting (no server-side processing needed)
- HTTPS support recommended
- Gzip compression recommended

## Academic/Educational Considerations

### Institutional Hosting
- Check if your university offers web hosting
- Many institutions provide free hosting for academic projects
- Consider open access requirements for research projects

### Licensing and Attribution
- Ensure proper attribution for all data sources
- Consider adding a license file (CC BY-SA recommended for academic work)
- Include citation information for researchers

## Troubleshooting Common Issues

### CORS Errors
If you encounter Cross-Origin Resource Sharing errors:
- Ensure all files are served from the same domain
- Use a proper web server (not file:// protocol)

### Large File Sizes
If hosting providers complain about file sizes:
- Consider using Git LFS for large files
- Compress MEI files
- Use external storage for large datasets

### Loading Performance
If the site loads slowly:
- Enable compression on your server
- Use a CDN
- Lazy load MEI files

## Next Steps After Deployment

1. **Test thoroughly** on different devices and browsers
2. **Set up analytics** to track usage
3. **Create documentation** for users
4. **Share with academic community**
5. **Gather feedback** for improvements

## Support and Community

### Getting Help
- GitHub Issues (if using GitHub Pages)
- Hosting provider support
- Web development communities (Stack Overflow, Reddit)

### Sharing Your Work
- Academic conferences
- Digital humanities communities
- Cultural heritage organizations
- Music education networks

---

**Ready to deploy?** Choose your preferred method and follow the step-by-step instructions above. The platform is well-prepared for web deployment with all necessary files and optimizations in place.
