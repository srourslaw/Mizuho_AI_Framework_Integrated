# Google Analytics Setup Guide

## Quick Setup (2 minutes)

### Step 1: Get Your Tracking ID
1. Go to [analytics.google.com](https://analytics.google.com)
2. Sign in with your Google account
3. Click "Start measuring"
4. Create an account name (e.g., "Mizuho Dashboard")
5. Create a property name (e.g., "Mizuho AI Discovery")
6. Select your country/region and currency
7. Choose "Web" platform
8. Enter your website URL: `https://srourslaw.github.io/Mizuho_AI_Framework_Integrated/`
9. Copy your **Measurement ID** (looks like `G-XXXXXXXXXX`)

### Step 2: Replace Placeholder ID
Find and replace `G-MIZUHO2025` with your real Measurement ID in these files:
- `index.html` (line 9)
- `dashboards/mizuho-use-cases.html` (line 9)
- `dashboards/two-week-discovery.html` (line 9)
- `dashboards/framework-visualization.html` (line 9)
- `dashboards/regional-expansion.html` (line 9)

### Step 3: Commit Changes
```bash
git add .
git commit -m "Update Google Analytics tracking ID"
git push
```

## What You'll See

### Real-Time Tracking
- Live visitor count
- Active pages being viewed
- Geographic location of visitors
- Traffic sources (GitHub, direct, email, etc.)

### Historical Data
- Daily/weekly/monthly visitor trends
- Most popular pages
- Session duration and engagement
- Device and browser information

### GitHub-Specific Insights
- Track clicks from GitHub repository
- Identify referral traffic from github.com
- Monitor conversion from README to dashboard

## Access Your Analytics
Visit [analytics.google.com](https://analytics.google.com) to view all tracking data.

**Note**: Analytics data may take 24-48 hours to start appearing after setup.