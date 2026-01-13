# NestPlan Retirement Calculator

Professional retirement planning tool with Monte Carlo simulation, tax optimization, and scenario management.

**Live Site:** https://topshopnation.com/nestplan/  
**Business Entity:** CoreForge LLC  
**Current Version:** v4.3 (Mobile-Optimized)

## Features

### FREE Tier
- ✅ Basic retirement projections with tax calculations
- ✅ HSA tracking and cost basis calculations
- ✅ Spouse support with separate accounts
- ✅ 1 saved scenario
- ❌ No charts (Total Assets Over Time, Asset Allocation)
- ❌ No year-by-year table
- ❌ No Monte Carlo simulation
- ❌ No PDF export

### PRO Tier ($4.99 one-time or $1.99/month)
- ✅ Monte Carlo simulation (1,000 runs)
- ✅ Total Assets Over Time chart
- ✅ Asset Allocation chart
- ✅ Year-by-Year projection table
- ✅ PDF export with full reports
- ✅ JSON import/export for backups
- ✅ Up to 12 saved scenarios

## Tech Stack
- React 18 (CDN-based, no build process)
- Tailwind CSS v3
- Chart.js 4.4
- jsPDF 2.5
- localStorage for data persistence
- Single HTML file architecture

## File Structure
```
nestplan/
├── index.html          # Main calculator app (v4.3)
├── privacy.html        # Privacy policy (required for App Store)
├── terms.html          # Terms of service
├── support.html        # Support/FAQ page
└── icons/             # App icons for iOS (76-1024px)
```

## Local Development

The app runs as a single HTML file with no build process:

1. Clone the repo
2. Open `nestplan/index.html` in a browser
3. Edit and refresh to test changes

## Deployment

**Current Setup:** GitHub Pages → Namecheap DNS

The site auto-deploys from the `main` branch when you push changes.

### Manual Deploy to Unraid (for testing)
```bash
scp ~/Downloads/index.html root@192.168.1.10:/mnt/cache/appdata/nestplan/
ssh root@192.168.1.10 "docker restart nestplan"
```

## iOS App Roadmap

**Status:** Web app complete, iOS wrapper in progress

Next steps:
1. ✅ Legal pages (Privacy, Terms) - DONE
2. ⏳ Capacitor iOS wrapper
3. ⏳ StoreKit 2 in-app purchase implementation
4. ⏳ TestFlight beta testing
5. ⏳ App Store submission

**Target Timeline:** 3-4 weeks to App Store ready

## License

© 2026 CoreForge LLC. All rights reserved.

## Contact

For support: [Email Support](mailto:support@topshopnation.com)
