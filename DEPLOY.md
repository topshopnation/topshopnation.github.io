# Deployment Guide

## GitHub Pages
This site is hosted on GitHub Pages and deploys automatically from the `main` branch.

**Live URLs:**
- Main site: https://topshopnation.com
- NestPlan: https://topshopnation.com/nestplan/

## How to Update

### Via GitHub Web Interface
1. Navigate to the file you want to edit
2. Click the pencil icon (Edit)
3. Make changes
4. Commit changes
5. Wait 1-2 minutes for deployment

### Via Git
```bash
git clone https://github.com/topshopnation/topshopnation.github.io.git
cd topshopnation.github.io
# Make changes
git add .
git commit -m "Description of changes"
git push origin main
```

## File Structure
```
/
├── index.html              # Landing page
├── CNAME                   # Domain config
└── nestplan/
    ├── index.html          # App landing
    ├── privacy.html        # Privacy policy
    ├── terms.html          # Terms of service
    └── support.html        # Support page
```

## Notes
- Changes deploy automatically within 1-2 minutes
- HTTPS is enforced
- Custom domain configured via CNAME
