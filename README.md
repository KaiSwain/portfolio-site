# Portfolio Website Template

A modern, responsive portfolio website for a junior software developer. Features smooth animations, mobile-friendly design, and easy customization.

## 🚀 Features

- **Responsive Design**: Works perfectly on desktop, tablet, and mobile devices
- **Smooth Animations**: Engaging scroll animations and transitions
- **Modern UI**: Clean, professional design with gradient accents
- **Easy to Customize**: Simple structure for quick personalization
- **Sections Include**:
  - Hero/Landing section with profile picture
  - About Me with stats
  - Projects showcase
  - Skills & Technologies
  - Contact form
  - Social media links

## 📁 Project Structure

```
portfolio-site/
├── index.html      # Main HTML file
├── styles.css      # All styling and responsive design
├── script.js       # Interactive features and animations
└── README.md       # This file
```

## 🎨 How to Customize

### 1. Personal Information

Open `index.html` and replace the following:

- **Line 8**: Change `Your Name` in the title tag
- **Line 16**: Update the logo text `<YourName />`
- **Line 30**: Update your name in the hero title
- **Line 31**: Customize your role/title
- **Line 32-35**: Write your own introduction
- **Line 40-48**: Update social media links (GitHub, LinkedIn, Twitter)

### 2. Adding Your Profile Picture

**Hero Section (Large circular image):**
1. Save your profile picture as `profile.jpg` in the same folder
2. In `index.html`, find line 52-56 (the profile-image-placeholder div)
3. Replace it with:
```html
<div class="hero-image">
    <img src="profile.jpg" alt="Your Name" style="width: 400px; height: 400px; border-radius: 50%; object-fit: cover; box-shadow: 0 20px 60px rgba(99, 102, 241, 0.3);">
</div>
```

**About Section Image:**
1. Save another image as `about-image.jpg`
2. In `index.html`, find line 67-72 (about-image-placeholder div)
3. Replace it with:
```html
<div class="about-image">
    <img src="about-image.jpg" alt="About me" style="width: 100%; height: 400px; border-radius: 15px; object-fit: cover; box-shadow: 0 10px 40px rgba(99, 102, 241, 0.2);">
</div>
```

### 3. Adding Project Screenshots

For each project (there are 3 by default):

1. Save your project screenshot (e.g., `project1.jpg`, `project2.jpg`, `project3.jpg`)
2. Find the project-image-placeholder divs (around lines 106, 128, 150)
3. Replace each with:
```html
<div class="project-image">
    <img src="project1.jpg" alt="Project Name" style="width: 100%; height: 250px; object-fit: cover;">
</div>
```

### 4. Update Project Information

For each project card:
- **Project Name**: Update the `<h3>` tag
- **Description**: Update the paragraph describing the project
- **Technologies**: Modify the tags in `project-tags` div
- **Links**: Update the href attributes for Live Demo and Code links

Example (around line 108):
```html
<h3>Weather Dashboard</h3>
<p>A React-based weather application that shows real-time weather data using OpenWeatherMap API.</p>
<div class="project-tags">
    <span class="tag">React</span>
    <span class="tag">API</span>
    <span class="tag">CSS</span>
</div>
<div class="project-links">
    <a href="https://your-demo-link.com" class="project-link" target="_blank">
        <i class="fas fa-external-link-alt"></i> Live Demo
    </a>
    <a href="https://github.com/yourusername/project" class="project-link" target="_blank">
        <i class="fab fa-github"></i> Code
    </a>
</div>
```

### 5. Update Skills

In the Skills section (around line 170), customize the technologies you know:

```html
<div class="skill-category">
    <h3><i class="fas fa-code"></i> Frontend</h3>
    <ul>
        <li><i class="fab fa-html5"></i> HTML5</li>
        <li><i class="fab fa-css3-alt"></i> CSS3</li>
        <li><i class="fab fa-js"></i> JavaScript</li>
        <li><i class="fab fa-react"></i> React</li>
    </ul>
</div>
```

Add or remove skills as needed. Icons are from Font Awesome.

### 6. Update Contact Information

Around line 214, update your contact details:

```html
<div class="contact-item">
    <i class="fas fa-envelope"></i>
    <div>
        <h4>Email</h4>
        <a href="mailto:your.email@example.com">your.email@example.com</a>
    </div>
</div>
```

Do the same for phone and location.

### 7. Update About Section Stats

Around line 82, customize your statistics:

```html
<div class="stat">
    <h4>15+</h4>
    <p>Projects Completed</p>
</div>
```

### 8. Customize Colors

To change the color scheme, edit the CSS variables in `styles.css` (lines 9-18):

```css
:root {
    --primary-color: #6366f1;      /* Main brand color */
    --secondary-color: #8b5cf6;    /* Secondary brand color */
    --accent-color: #ec4899;       /* Accent color */
    /* ... */
}
```

## 🌐 Deployment

### Option 1: GitHub Pages (Free)
1. Create a GitHub repository
2. Push your code to the repository
3. Go to Settings > Pages
4. Select your branch (usually `main`) and save
5. Your site will be live at `https://yourusername.github.io/repository-name`

### Option 2: Netlify (Free)
1. Create an account at [netlify.com](https://netlify.com)
2. Drag and drop your project folder
3. Your site will be live instantly with a custom URL

### Option 3: Vercel (Free)
1. Create an account at [vercel.com](https://vercel.com)
2. Import your GitHub repository or upload files
3. Deploy with one click

## 💡 Tips

1. **Images**: Use optimized images (compress them) for faster loading
2. **Image Sizes**: 
   - Profile picture: 400x400px recommended
   - Project screenshots: 800x600px or similar aspect ratio
   - About image: 600x800px or similar
3. **Alt Text**: Always add descriptive alt text to images for accessibility
4. **Testing**: Test your site on different devices and browsers
5. **Contact Form**: The contact form currently shows an alert. To make it functional, you'll need to integrate with a service like:
   - [Formspree](https://formspree.io/)
   - [EmailJS](https://www.emailjs.com/)
   - [Netlify Forms](https://www.netlify.com/products/forms/)

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## 🛠️ Future Enhancements

Consider adding:
- Blog section
- Dark mode toggle
- Animation on scroll using libraries like AOS
- Backend for contact form
- Resume download button
- Testimonials section
- More projects with pagination

## 📝 License

Feel free to use this template for your own portfolio!

## 🤝 Need Help?

If you have questions about customization:
1. Check the comments in the HTML, CSS, and JS files
2. Refer to this README
3. The structure is straightforward - each section is clearly marked

---

**Good luck with your portfolio! 🚀**
