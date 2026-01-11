# Laamu Apex Sports Academy (LASA) Website

A modern, professional, and responsive website for Laamu Apex Sports Academy in Laamu Atoll, Maldives.

## 🌟 Features

- **Modern & Professional Design**: Eye-catching gradient hero with animated particles
- **Fully Responsive**: Seamless experience on desktop, tablet, and mobile devices
- **Interactive Elements**: 
  - Smooth scrolling navigation
  - Animated counters for statistics
  - Scroll-triggered animations
  - Parallax effects
  - Hover interactions
- **Comprehensive Sections**:
  - Dynamic hero with academy stats
  - About section with key features
  - Achievements showcase
  - Detailed sports programs
  - Image gallery
  - Testimonials
  - Contact form
- **Social Media Integration**: Direct links to Facebook and other platforms
- **Performance Optimized**: Fast loading with smooth animations

## 📁 File Structure

```
LASA/
├── index.html          # Main HTML file
├── styles.css          # All styling and animations
├── script.js           # Interactive functionality
└── README.md          # Documentation
```

## 🎨 Sections Overview

### 1. **Hero Section**
- Gradient background with animated particles
- Academy statistics (100+ Athletes, 5+ Sports, Expert Coaches)
- Call-to-action buttons
- Premium badge

### 2. **About Section**
- Mission statement
- Key features with icons:
  - Professional Coaching
  - Modern Facilities
  - Community Focus
  - Excellence

### 3. **Achievements**
- Championship wins
- Certified programs
- Top athletes
- Community impact

### 4. **Programs** (4 Main Programs)
- ⚽ Football Training
- 🏀 Basketball Program
- 🏃 Athletics & Track
- 🏐 Multi-Sport Development

### 5. **Gallery**
- 6 image slots ready for photos
- Hover effects
- Lightbox-ready structure

### 6. **Testimonials**
- 3 testimonial cards
- 5-star ratings
- Parent and athlete feedback

### 7. **Contact Section**
- Contact information
- Inquiry form with program selection
- Social media links
- Location details

## 📸 Adding Real Photos and Logo

### Download the Academy Logo:

1. **Visit Facebook**: https://www.facebook.com/people/Laamu-Apex-Sports-Academy/100090281827371/

2. **Download the profile picture (logo)**:
   - Right-click on the profile picture → "Open image in new tab"
   - Right-click on the image → "Save image as..."
   - Save as `lasa-logo.png` in the `images` folder
   - The website will automatically use it!

   *Alternative*: See `images/DOWNLOAD_LOGO_INSTRUCTIONS.txt` for detailed steps

3. **Download photos** for:
   - Hero background (action sports photo)
   - About section image
   - 6 Gallery images (training sessions, events, facilities)

3. **Create an `images` folder** in the LASA directory

4. **Save images** as:
   - `hero-bg.jpg` (1920x1080px recommended)
   - `about.jpg` (800x600px)
   - `gallery-1.jpg` through `gallery-6.jpg` (800x600px each)

5. **Update HTML** - Replace placeholder sections:

```html
<!-- Hero Background -->
<section id="home" class="hero" style="background-image: linear-gradient(rgba(0,0,0,0.4), rgba(0,0,0,0.4)), url('images/hero-bg.jpg'); background-size: cover; background-position: center;">

<!-- About Image -->
<div class="about-image">
    <img src="images/about.jpg" alt="LASA Academy" style="width: 100%; border-radius: 10px;">
</div>

<!-- Gallery Images -->
<div class="gallery-item">
    <img src="images/gallery-1.jpg" alt="Training Session">
</div>
```

### Recommended Photo Types:

- **Hero**: Dynamic action shot (football match, athletes training)
- **About**: Group photo of coaches and athletes
- **Gallery**:
  1. Football training session
  2. Basketball practice
  3. Athletics/running event
  4. Team celebration/achievement
  5. Facilities/equipment
  6. Community event/tournament

## 🎯 Customization Guide

### Update Contact Information

In `index.html`, find the contact section and update:

```html
<div class="info-item">
    <i class="fas fa-phone"></i>
    <div>
        <h4>Phone</h4>
        <p>+960 XXX-XXXX</p>  <!-- Add real phone -->
    </div>
</div>

<div class="info-item">
    <i class="fas fa-envelope"></i>
    <div>
        <h4>Email</h4>
        <p>info@laamuapexsports.com</p>  <!-- Update email -->
    </div>
</div>
```

### Add Social Media Links

```html
<a href="https://www.instagram.com/your-profile" target="_blank">
    <i class="fab fa-instagram"></i>
</a>
<a href="https://twitter.com/your-profile" target="_blank">
    <i class="fab fa-twitter"></i>
</a>
```

### Modify Colors

In `styles.css`, update the CSS variables:

```css
:root {
    --primary-color: #e74c3c;      /* Main brand color */
    --secondary-color: #2c3e50;    /* Secondary color */
    --accent-color: #3498db;       /* Accent color */
}
```

### Add More Programs

Duplicate a program card in the HTML:

```html
<div class="program-card">
    <div class="program-icon">
        <i class="fas fa-swimmer"></i>
    </div>
    <h3>Swimming Program</h3>
    <p>Description here...</p>
    <ul>
        <li>Training point 1</li>
        <li>Training point 2</li>
    </ul>
    <a href="#contact" class="program-link">Enroll Now <i class="fas fa-arrow-right"></i></a>
</div>
```

## 🚀 Launch Instructions

### Local Testing:
1. Simply open `index.html` in any modern web browser
2. Test all sections and interactions
3. Check mobile responsiveness (use browser dev tools)

### Web Hosting Options:

1. **Free Hosting**:
   - GitHub Pages (free, easy setup)
   - Netlify (free tier with custom domain)
   - Vercel (free for personal projects)

2. **Premium Hosting** (for custom domain):
   - HostGator
   - Bluehost
   - SiteGround

### Quick Deploy to GitHub Pages:

```bash
# Initialize git repository
git init
git add .
git commit -m "Initial LASA website"

# Create repository on GitHub, then:
git remote add origin https://github.com/yourusername/lasa-website.git
git push -u origin main

# Enable GitHub Pages in repository settings
# Your site will be live at: https://yourusername.github.io/lasa-website
```

## 📧 Contact Form Integration

The contact form currently displays an alert. To make it functional:

### Option 1: FormSpree (Easy, Free)
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

### Option 2: EmailJS (Free, JavaScript-based)
```javascript
emailjs.send("service_id", "template_id", {
    name: name,
    email: email,
    message: message
});
```

### Option 3: Backend Integration
- Use PHP, Node.js, or Python backend
- Set up email service (SendGrid, Mailgun)

## 🔧 Technical Details

### Technologies Used:
- HTML5
- CSS3 (with CSS Variables, Flexbox, Grid)
- Vanilla JavaScript
- Font Awesome 6.4.0 (for icons)

### Browser Compatibility:
- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

### Performance Features:
- Optimized animations (60fps)
- Lazy-loaded elements
- Efficient CSS transitions
- Minimal JavaScript footprint

## 📱 Mobile Responsiveness

The website is fully responsive with breakpoints at:
- Desktop: > 1200px
- Tablet: 768px - 1200px
- Mobile: < 768px
- Small Mobile: < 480px

## ✅ Checklist for Launch

- [ ] Add real photos from Facebook/events
- [ ] Update contact information
- [ ] Test contact form
- [ ] Add Instagram/Twitter handles
- [ ] Test on multiple devices
- [ ] Check all links work
- [ ] Optimize images for web
- [ ] Set up domain name (if applicable)
- [ ] Deploy to hosting
- [ ] Test live site
- [ ] Set up Google Analytics (optional)
- [ ] Submit to Google Search Console

## 🎓 Future Enhancements

Consider adding:
- Blog section for news and updates
- Online registration system
- Payment integration for program fees
- Video gallery/YouTube integration
- Events calendar
- Member login area
- Photo gallery with lightbox
- Live chat support
- Multi-language support (Dhivehi/English)

## 📞 Support

For questions or updates, contact the academy:
- Facebook: https://www.facebook.com/people/Laamu-Apex-Sports-Academy/100090281827371/
- Location: Laamu Atoll, Maldives

## 📄 License

This website is created for Laamu Apex Sports Academy.

---

**Built with ❤️ for Laamu Apex Sports Academy**
*Building Champions, Shaping Futures*

🏆 Excellence in Sports Education 🏆
