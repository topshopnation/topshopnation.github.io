# NestPlan Web Pages - Changelog

## January 13, 2026 - v1.1

### 🔧 Changed
- **Removed all pricing information** from web pages
  - Support FAQ: "Pricing is available in the app"
  - Privacy Policy: Removed dollar amounts
  - Terms of Service: Generic subscription language
  - README: No pricing in feature table
  
**Reason:** Allows App Store pricing changes without updating web pages

### 📝 Updated Pages
- `/nestplan/privacy.html` - Removed "$4.99/year" references
- `/nestplan/terms.html` - Removed specific pricing details
- `/nestplan/support.html` - Made pricing FAQ generic
- `README.md` - Updated feature comparison without pricing

### ✅ Kept Features
- Ad monetization details (Google AdMob)
- FREE vs PRO feature comparison
- Legal disclaimers and privacy info
- Support contact information

### 📦 What's in This Package
```
github-package/
├── CNAME                    # Domain config
├── README.md                # Project docs (pricing removed)
├── .gitignore              # Git ignore rules
├── DEPLOY.md               # Deployment instructions (NEW)
├── CHANGELOG.md            # This file (NEW)
├── index.html              # CoreForge landing page
└── nestplan/
    ├── index.html          # NestPlan landing
    ├── privacy.html        # Updated (no pricing)
    ├── terms.html          # Updated (no pricing)
    └── support.html        # Updated (no pricing)
```

---

## January 12, 2026 - v1.0

### 🎉 Initial Release
- Created GitHub Pages site
- Configured custom domain (topshopnation.com)
- Added legal pages (Privacy, Terms, Support)
- Created NestPlan landing page
- Enabled HTTPS
