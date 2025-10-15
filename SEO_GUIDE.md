# SEO Optimization Guide

This document explains the SEO improvements made to make your website searchable on Google and other search engines.

## Changes Made

### 1. robots.txt
**Location:** `robots.txt` (root directory)

This file tells search engines which pages they can crawl. We've configured it to:
- Allow all search engines to crawl the entire site
- Point to the sitemap location

### 2. sitemap.xml
**Location:** `sitemap.xml` (root directory)

A sitemap helps search engines discover all your pages. It includes:
- Homepage (https://garyntan.github.io/)
- CV PDF
- Job Market Paper PDF

**Priority levels:**
- Homepage: 1.0 (highest)
- Job Market Paper: 0.9 (very important)
- CV: 0.8 (important)

### 3. Enhanced HTML Meta Tags

#### Primary Meta Tags
- **Description**: Rich, keyword-optimized description of your academic profile
- **Keywords**: Relevant search terms (Economics, Labor Economics, NDIS, etc.)
- **Author**: Your name for attribution
- **Robots**: Explicit instruction to index and follow links

#### Open Graph Tags (for Social Media)
Enables rich previews when sharing on Facebook, LinkedIn, etc.:
- Title, description, and image preview
- Proper URL and content type

#### Twitter Cards
Optimizes how your site appears when shared on Twitter

#### Canonical URL
Prevents duplicate content issues by specifying the primary URL

#### Structured Data (JSON-LD)
Schema.org Person markup that helps search engines understand:
- Your role and affiliation
- Your education background
- Your research areas
- Links to your professional profiles

## Next Steps to Improve Search Visibility

### 1. Submit to Google Search Console
1. Go to [Google Search Console](https://search.google.com/search-console)
2. Add your property: `https://garyntan.github.io/`
3. Verify ownership (GitHub Pages verification)
4. Submit your sitemap: `https://garyntan.github.io/sitemap.xml`
5. Request indexing for your homepage

### 2. Submit to Bing Webmaster Tools
1. Go to [Bing Webmaster Tools](https://www.bing.com/webmasters)
2. Add and verify your site
3. Submit sitemap

### 3. Build Backlinks
- Add your website to your university profile page
- Link from your Google Scholar profile
- Link from your LinkedIn profile (already done)
- Add to academic networking sites (ResearchGate, Academia.edu)
- Include in email signatures

### 4. Regular Updates
Search engines favor regularly updated content:
- Update the "Last updated" date when you make changes
- Update the sitemap.xml lastmod dates
- Add new papers or publications as they come out

### 5. Monitor Performance
After deployment, monitor your search performance:
- Use Google Search Console to see which queries bring users
- Check which pages are indexed
- Monitor for any crawl errors

## How Long Until I Appear in Search?

- **First crawl**: Usually within a few days after submitting sitemap
- **Full indexing**: Can take 1-4 weeks
- **Ranking improvements**: May take several weeks to months as Google evaluates content quality and relevance

## Testing Your SEO

### Check if indexed
Search Google for:
```
site:garyntan.github.io
```

### Test structured data
1. Go to [Google Rich Results Test](https://search.google.com/test/rich-results)
2. Enter your URL: `https://garyntan.github.io/`
3. Check that the Person schema is recognized

### Test robots.txt
Visit: `https://garyntan.github.io/robots.txt`

### Test sitemap
Visit: `https://garyntan.github.io/sitemap.xml`

## Additional Tips

### Content Optimization
Your site already has good content, but consider:
- Using heading tags (H1, H2, H3) properly (already done)
- Including relevant keywords naturally in your text
- Making sure all images have descriptive alt text (already done)

### Technical SEO
- ✅ Mobile-friendly design (already responsive)
- ✅ Fast loading (static HTML, minimal dependencies)
- ✅ HTTPS enabled (GitHub Pages default)
- ✅ Clean URLs (no query parameters)

### Academic-Specific SEO
- Ensure your papers have proper citations
- Include JEL codes (already done)
- Add keywords for your research areas
- Link to your ORCID profile if you have one

## Maintenance

Update the sitemap.xml whenever you:
- Add new publications
- Update your CV
- Add new pages

Update the lastmod date in sitemap.xml to reflect changes.

## Questions?

If you have questions about SEO or need to make adjustments, refer to:
- [Google Search Central](https://developers.google.com/search)
- [Schema.org](https://schema.org/) for structured data
- [Sitemaps.org](https://www.sitemaps.org/) for sitemap specifications
