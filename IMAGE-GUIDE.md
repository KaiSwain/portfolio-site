# How to Add Images to Your Project Showcases

## Quick Guide for Adding Screenshots

### For Teacher Portal (teacher-portal.html)

1. **Save your images** in the `/home/kaifer/workspace/portfolio-site/` folder with these names:
   - `teacher-portal-main.png` - Main hero screenshot
   - `teacher-portal-dashboard.png` - Dashboard view
   - `teacher-portal-progress.png` - Student progress tracking
   - `teacher-portal-pdf.png` - PDF generation feature
   - `teacher-portal-ai.png` - AI insights
   - `teacher-portal-files.png` - File management
   - `teacher-portal-mobile.png` - Mobile responsive view

2. **Replace the placeholder divs** in `teacher-portal.html`:

   For the **main screenshot** (around line 53), replace:
   ```html
   <div class="screenshot-placeholder main">
       <i class="fas fa-image"></i>
       <p>Add your main screenshot here</p>
       <span class="helper-text">Drag and drop your main dashboard screenshot (recommended size: 1200x700px)</span>
   </div>
   ```
   
   With:
   ```html
   <img src="teacher-portal-main.png" alt="Teacher Portal Dashboard" style="width: 100%; border-radius: 15px; box-shadow: 0 20px 60px rgba(0, 0, 0, 0.2);">
   ```

   For **gallery screenshots** (starting around line 135), replace each placeholder div like this:
   ```html
   <div class="screenshot-placeholder">
       <i class="fas fa-image"></i>
       <p>Dashboard View</p>
       <span class="helper-text">Add dashboard screenshot</span>
   </div>
   ```
   
   With:
   ```html
   <img src="teacher-portal-dashboard.png" alt="Dashboard View" style="width: 100%; height: 300px; object-fit: cover;">
   ```

### Quick Replace Pattern

For any screenshot placeholder, use this pattern:
```html
<!-- OLD (remove this) -->
<div class="screenshot-placeholder">
    <i class="fas fa-image"></i>
    <p>Text</p>
    <span class="helper-text">Help text</span>
</div>

<!-- NEW (replace with this) -->
<img src="your-image-name.png" alt="Descriptive alt text" style="width: 100%; height: 300px; object-fit: cover;">
```

### Image Size Recommendations

- **Main hero images**: 1200x700px or 1920x1080px
- **Gallery screenshots**: 800x600px or similar aspect ratio
- **Format**: PNG or JPG
- **Optimization**: Compress images to keep file size under 500KB each

### For Projects 2 & 3

Follow the same pattern in `project-2.html` and `project-3.html`:
1. Save your images with descriptive names
2. Replace the `<div class="screenshot-placeholder">` with `<img src="...">` tags
3. Keep the alt text descriptive for accessibility

### Example: Complete Gallery Item

```html
<div class="gallery-item">
    <img src="teacher-portal-dashboard.png" alt="Teacher Dashboard" style="width: 100%; height: 300px; object-fit: cover;">
    <div class="gallery-caption">
        <h3>Dashboard Overview</h3>
        <p>Comprehensive dashboard showing student metrics, recent activities, and quick actions.</p>
    </div>
</div>
```

## Testing Your Images

After adding images:
1. Save the files
2. Refresh your browser at `http://localhost:8080`
3. Click on "View Details" for any project
4. Check that all images load correctly

## Need Help?

- Make sure image file names match exactly (case-sensitive)
- All images should be in the same folder as your HTML files
- If images don't show, check the browser console (F12) for errors
