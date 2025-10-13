# Quick Start Guide

## Customization Checklist

Follow these steps to personalize your economics job market paper website:

### 1. Update Personal Information (index.html)

**Lines to modify:**
- Line 7: Change page title from "Your Name" to your actual name
- Line 15: Replace "Your Name" with your name
- Line 16: Update "Economics PhD Candidate" with your title
- Line 17: Replace "University Name | Department of Economics" with your affiliation
- Lines 19-21: Update email, LinkedIn URL, and CV link

### 2. Update Job Market Paper Section (index.html)

**Lines to modify:**
- Line 27: Replace "Your Paper Title: A Comprehensive Analysis of Economic Phenomena" with your actual paper title
- Line 30: Update href to point to your paper PDF file
- Lines 36-41: Replace the abstract with your paper's abstract
- Line 43: Update keywords
- Line 46: Update JEL codes

### 3. Update About Me Section (index.html)

**Lines to modify:**
- Lines 53-61: Replace placeholder text with your actual bio

### 4. Update Research Interests (index.html)

**Lines to modify:**
- Lines 67-69: Update with your actual research fields

### 5. Update Additional Papers (index.html)

**Lines to modify:**
- Lines 75-84: Add your working papers or remove this section if not needed

### 6. Add Your PDF Files

Place these files in the same directory:
- `paper.pdf` - Your job market paper
- `cv.pdf` - Your curriculum vitae
- Any additional working paper PDFs mentioned in the HTML

### 7. Add Paper Images (Optional but Recommended)

Add visual elements to make your papers stand out:
- `paper-image.jpg` - An image for your job market paper (e.g., key figure, chart, or diagram from the paper)
- `working-paper-1-image.jpg` - Image for working paper 1
- `working-paper-2-image.jpg` - Image for working paper 2

**Image Guidelines:**
- **Recommended source size**: 400x300 pixels (or similar 4:3 ratio) for job market paper, 240x180 pixels for working papers
- **Display size**: Images will be displayed at 200px width for job market paper and 120px width for working papers, scaled proportionally
- **Format**: JPG or PNG
- **Content ideas**: Key graphs, charts, maps, or visual summaries from your research
- **Tip**: Export a key figure from your paper at high resolution (2x the display size for retina screens) and crop appropriately

If you don't want to include images, you can remove the image elements from the HTML or leave the placeholders - they will show broken image icons which users can ignore.

### 8. Deploy Your Website

**Option A: GitHub Pages (Recommended)**
1. Repository already exists at https://github.com/garyntan/website
2. Go to repository Settings → Pages
3. Select "Deploy from a branch"
4. Choose "main" branch and "/" (root) folder
5. Click Save
6. Your site will be available at: https://garyntan.github.io/

**Option B: Custom Domain**
1. Upload files to your web hosting service
2. Point your domain to the hosting service
3. Access via your custom domain

## Testing Locally

To test your changes before deploying:

```bash
# Navigate to the website directory
cd /path/to/website

# Start a local web server (Python 3)
python3 -m http.server 8000

# Or using Python 2
python -m SimpleHTTPServer 8000

# Or using Node.js (if you have it)
npx http-server

# Open in browser
# http://localhost:8000
```

## Tips

1. **Keep it simple**: Don't add too much content. Focus on your job market paper.
2. **Professional photo**: Consider adding a professional headshot in the header.
3. **Use compelling visuals**: Add images showing key figures or results from your papers to make them more engaging.
4. **Update regularly**: Keep your abstract and CV up to date.
5. **Test links**: Make sure all PDF links work before sending to potential employers.
6. **Mobile check**: Always check how your site looks on mobile devices.

## Need Help?

- The HTML structure is in `index.html`
- All styling is in `styles.css`
- Refer to `README.md` for detailed documentation
