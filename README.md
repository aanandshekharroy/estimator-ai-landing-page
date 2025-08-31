# Estimator AI Landing Page

A simple, mobile-responsive landing page built for GitHub Pages.

## Features

✅ **Mobile Responsive Design** - Looks great on all devices  
✅ **Modern CSS Styling** - Gradient backgrounds and smooth animations  
✅ **Video Embed Support** - Showcase your product with embedded video  
✅ **Call-to-Action Button** - Direct users to your Google Form  
✅ **Fast Loading** - Single HTML file with inline CSS  

## Setup for GitHub Pages

1. **Push to GitHub**: Upload these files to your GitHub repository
2. **Enable GitHub Pages**: 
   - Go to your repo's Settings
   - Scroll down to "Pages" section
   - Select "Deploy from a branch"
   - Choose "main" branch and "/ (root)" folder
   - Save the settings
3. **Your site will be live at**: `https://[your-username].github.io/[repo-name]`

## Customization Required

Before going live, you'll need to update these items in `index.html`:

### 1. Video File (Line ~159)
Add your `.mov` video file to the repository and update the filename:
```html
<source src="your-product-demo.mov" type="video/quicktime">
```

**Video Setup Steps:**
1. **Add video to repo**: Upload your `.mov` file to the root directory or create a `videos/` folder
2. **Update filename**: Change `your-product-demo.mov` to match your actual filename
3. **Optional**: Convert to `.mp4` for better browser compatibility (the HTML includes both formats)
4. **File size**: Keep video under 100MB (GitHub's file size limit) - consider compressing if needed

### 2. Google Form Link (Line ~100)
Replace the `#` in the button href with your Google Form URL:
```html
<a href="https://forms.google.com/your-form-link" class="cta-button"
```

### 3. Content (Optional)
- Update the title "Estimator AI" if needed
- Modify the description text to match your product
- Change the page title in the `<title>` tag

## File Structure

```
estimator-ai-landing-page/
├── index.html          # Main landing page
└── README.md          # This file
```

## Mobile Responsiveness

The page automatically adapts to different screen sizes:
- **Desktop**: Full-width layout with large text
- **Tablet** (768px and below): Adjusted spacing and font sizes
- **Mobile** (480px and below): Stacked layout with full-width button

## Support

This is a static HTML page that works out of the box with GitHub Pages. No build process or dependencies required!
