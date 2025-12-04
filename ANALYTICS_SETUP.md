# Analytics Setup Guide

This website now includes Google Analytics 4 (GA4) tracking to monitor site visits and PDF downloads.

## What's Been Added

The following analytics tracking has been implemented:

### 1. Page View Tracking
- **index.html**: Tracks all visits to your homepage
- **jmp_GT.html**: Tracks visits to the direct paper link (redirect page)

### 2. File Download Tracking
- **Job Market Paper (jmp_GT.pdf)**: Tracks downloads from the main paper button
- **CV (CV_GT.pdf)**: Tracks downloads from the CV link
- **Direct link downloads**: Tracks when someone accesses jmp_GT.html directly

## Setup Instructions

To activate analytics tracking, follow these steps:

### Step 1: Create a Google Analytics Account

1. Go to [Google Analytics](https://analytics.google.com/)
2. Sign in with your Google account
3. Click "Start measuring" or "Admin" (gear icon)

### Step 2: Create a Property

1. Click "Create Property" in the Admin section
2. Enter your property details:
   - **Property name**: "Garyn Tan Website" (or your preferred name)
   - **Reporting time zone**: Select your timezone
   - **Currency**: Select your preferred currency
3. Click "Next"
4. Fill in business details (optional for personal websites)
5. Click "Create"

### Step 3: Set Up a Data Stream

1. Select "Web" as your platform
2. Enter your website details:
   - **Website URL**: `https://garyntan.github.io`
   - **Stream name**: "Main Website" (or your preferred name)
3. Click "Create stream"
4. **IMPORTANT**: Copy your **Measurement ID** (it looks like `G-XXXXXXXXXX`)

### Step 4: Configure Your Website

Replace the placeholder Measurement ID in your HTML files:

1. Open **index.html**
2. Find this line (around line 35):
   ```html
   <script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
   ```
3. Replace `G-XXXXXXXXXX` with your actual Measurement ID
4. Find the next occurrence (around line 41):
   ```javascript
   gtag('config', 'G-XXXXXXXXXX');
   ```
5. Replace `G-XXXXXXXXXX` with your actual Measurement ID

6. Open **jmp_GT.html**
7. Repeat the same replacement for both occurrences of `G-XXXXXXXXXX`

### Step 5: Commit and Deploy

1. Commit your changes with the updated Measurement ID
2. Push to GitHub
3. Your analytics will start collecting data within 24-48 hours

## What You Can Track

Once set up, you'll be able to see:

### In Google Analytics Dashboard:

1. **Real-time users**: See who's on your site right now
2. **Page views**: Total visits to your homepage and redirect page
3. **User demographics**: Where your visitors are from (country, city)
4. **Traffic sources**: How people find your site (direct, search, referral)
5. **Device types**: Desktop vs mobile visitors

### Custom Events (File Downloads):

1. Go to Reports → Events in Google Analytics
2. Look for the `file_download` event
3. Click on it to see:
   - How many times jmp_GT.pdf was downloaded
   - How many times CV_GT.pdf was downloaded
   - Which link text users clicked (main paper button vs CV link)

## Creating Custom Reports

### To Create a Download Report:

1. Go to **Explore** in Google Analytics
2. Create a new "Free form" exploration
3. Add dimensions: `Event name`, `file_name`
4. Add metrics: `Event count`
5. Filter by: `Event name = file_download`

This will show you a detailed breakdown of all file downloads.

## Privacy Considerations

Google Analytics 4 is compliant with GDPR and other privacy regulations:
- It uses anonymized IP addresses by default
- No personal information is collected without user consent
- Data is aggregated for reporting

If you want to be more privacy-conscious, consider these alternatives:
- **Plausible Analytics**: Privacy-friendly, GDPR compliant, simple dashboard
- **Simple Analytics**: No cookies, privacy-first approach
- **Matomo**: Self-hosted option with full data ownership

To switch to an alternative, you would need to replace the Google Analytics code with the corresponding tracking code from your chosen provider.

## Testing Your Analytics

### Test Before Going Live:

1. Install the [Google Analytics Debugger](https://chrome.google.com/webstore/detail/google-analytics-debugger) Chrome extension
2. Visit your website locally or on GitHub Pages
3. Open Chrome DevTools (F12) → Console
4. Look for GA4 tracking messages to confirm events are firing

### Verify in Real-Time:

1. Go to Google Analytics → Reports → Real-time
2. Visit your website in a different browser
3. You should see yourself as a real-time visitor within seconds
4. Click on the PDF download link and watch the event appear

## Troubleshooting

### Not seeing any data?

1. **Check the Measurement ID**: Make sure you replaced `G-XXXXXXXXXX` with your actual ID in both files
2. **Wait 24-48 hours**: Initial data collection can take time
3. **Check Real-time reports**: These update immediately and can confirm tracking is working
4. **Browser extensions**: Ad blockers may prevent analytics from loading (this is normal for some visitors)
5. **HTTPS required**: GitHub Pages uses HTTPS by default, so this should work automatically

### Downloads not showing up?

1. Make sure the `onclick` event is properly added to the download links
2. Check that the `gtag` function is defined (view page source to confirm GA script loaded)
3. Look in the browser console for any JavaScript errors

## Additional Resources

- [Google Analytics 4 Help Center](https://support.google.com/analytics/answer/9304153)
- [GA4 Event Tracking Guide](https://support.google.com/analytics/answer/9267735)
- [GA4 Reports Overview](https://support.google.com/analytics/answer/9212670)

## Questions?

If you have questions or need help setting up analytics, you can:
- Check the [Google Analytics Community](https://support.google.com/analytics/community)
- Read the [GA4 documentation](https://developers.google.com/analytics/devguides/collection/ga4)
