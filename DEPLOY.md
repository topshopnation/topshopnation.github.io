# GitHub Pages Deployment Guide

## Current Status
✅ Website is live at https://topshopnation.com  
✅ GitHub Pages enabled and working  
✅ HTTPS enforced  
✅ Custom domain configured

## File Structure
```
topshopnation.github.io/
├── CNAME                    # Domain configuration (topshopnation.com)
├── README.md                # Project documentation
├── .gitignore              # Git ignore rules
├── index.html              # CoreForge Apps landing page
└── nestplan/               # NestPlan app directory
    ├── index.html          # NestPlan landing page
    ├── privacy.html        # Privacy policy
    ├── terms.html          # Terms of service
    └── support.html        # Support/FAQ page
```

## What Changed
🔧 **Removed all pricing information** from web pages:
- Support page now says "Pricing is available in the app"
- Privacy policy removed specific dollar amounts
- Terms of service removed pricing details
- README updated to remove pricing

This allows you to change App Store pricing without updating web pages.

## How to Deploy Updates

### Option 1: GitHub Web Interface (Easiest)
1. Go to https://github.com/topshopnation/topshopnation.github.io
2. Navigate to the file you want to update
3. Click the pencil icon (Edit)
4. Make your changes
5. Scroll down and click "Commit changes"
6. Wait 1-2 minutes for GitHub Pages to rebuild
7. Check https://topshopnation.com to see changes

### Option 2: Git Command Line (For Multiple Files)
```bash
# Clone the repo (first time only)
git clone https://github.com/topshopnation/topshopnation.github.io.git
cd topshopnation.github.io

# Make your changes to files

# Stage, commit, and push
git add .
git commit -m "Update description here"
git push origin main
```

### Option 3: Upload via GitHub (For This Package)
1. Go to https://github.com/topshopnation/topshopnation.github.io
2. Click "Add file" → "Upload files"
3. Drag all files from this package
4. When prompted about overwriting, confirm "Replace"
5. Scroll down and click "Commit changes"

## URLs
- Main site: https://topshopnation.com
- NestPlan landing: https://topshopnation.com/nestplan/
- Privacy: https://topshopnation.com/nestplan/privacy.html
- Terms: https://topshopnation.com/nestplan/terms.html
- Support: https://topshopnation.com/nestplan/support.html

## Notes
- GitHub Pages deploys automatically from the `main` branch
- Changes typically go live within 1-2 minutes
- HTTPS is enforced - HTTP traffic redirects to HTTPS
- Custom domain (topshopnation.com) is configured via CNAME file

## Troubleshooting
- **Changes not showing?** Wait 2-3 minutes, then hard refresh (Cmd+Shift+R on Mac)
- **404 errors?** Check that file paths match the structure above
- **Domain not working?** Verify CNAME file contains only: `topshopnation.com`
