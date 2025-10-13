# Economics Job Market Paper Website

A professional, clean website template for showcasing your economics job market paper.

## Features

- **Modern Design**: Clean, academic appearance suitable for economics job market candidates
- **Responsive Layout**: Works perfectly on desktop, tablet, and mobile devices
- **Easy to Customize**: Simple HTML and CSS structure for quick personalization
- **Professional Sections**: 
  - Header with name, affiliation, and contact information
  - Job market paper with abstract and download link
  - Research interests
  - Additional working papers
  - About section
- **Auto-updating Dates**: JavaScript automatically updates the current year and last modified date

## How to Use

1. **Customize the content** in `index.html`:
   - Replace "Your Name" with your actual name
   - Update university affiliation and contact information
   - Add your paper title and abstract
   - Update research interests and bio sections
   - Modify links to point to your actual PDF files

2. **Add your documents**:
   - Place your job market paper PDF as `paper.pdf` in the same directory
   - Add your CV as `cv.pdf`
   - (Optional) Add working papers with appropriate filenames

3. **Deploy the website**:
   - Upload all files to your web hosting service
   - Or use GitHub Pages: Enable GitHub Pages in repository settings and select the main branch

## File Structure

```
.
├── index.html       # Main HTML file with website structure
├── styles.css       # CSS styling for the website
├── README.md        # This file
├── paper.pdf        # Your job market paper (add this)
└── cv.pdf           # Your CV (add this)
```

## Customization Tips

### Colors
The main colors are defined in `styles.css`:
- Primary color: `#2980b9` (blue)
- Dark text: `#2c3e50`
- Light background: `#f5f5f5`

You can change these to match your preferences.

### Fonts
The default font is Georgia (serif) for an academic look. To change it, modify the `font-family` in `styles.css`.

### Sections
You can easily add or remove sections by editing the HTML. Each section follows this pattern:
```html
<section class="additional-section">
    <h2>Section Title</h2>
    <p>Content here...</p>
</section>
```

## Browser Support

This website works in all modern browsers:
- Chrome
- Firefox
- Safari
- Edge

## License

Feel free to use and modify this template for your personal academic website.
