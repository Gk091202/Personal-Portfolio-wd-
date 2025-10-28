# 🕷️ Spider-Man Themed Developer Portfolio

A modern, creative, and fully responsive web developer portfolio with a Spider-Man theme, featuring 3D effects, animations, and interactive elements.

## 🎨 Features

### Visual Effects

- ✨ **3D Tilt Effects** - Interactive cards with depth using Vanilla Tilt.js
- 🕸️ **Animated Spider Web Background** - Dynamic canvas-based web pattern
- 🌌 **Particle System** - Interactive particles that respond to mouse movement
- 💫 **Glitch Text Effect** - Cyberpunk-style glitch animation on hero title
- 🎭 **Loading Screen** - Spider symbol loader with pulsing animation
- 🌈 **Smooth Scroll Animations** - Elements fade in as you scroll
- ⚡ **Power Bars** - Animated skill level indicators
- 📊 **Counting Stats** - Numbers animate when scrolled into view

### Interactive Elements

- 🍔 **Responsive Hamburger Menu** - Mobile-friendly navigation
- 🎯 **Smooth Scroll Navigation** - Click nav links for smooth scrolling
- 📱 **Fully Responsive** - Works on all devices (mobile, tablet, desktop)
- ✉️ **Contact Form** - Functional form with validation
- ⬆️ **Scroll to Top Button** - Appears when scrolling down
- 🎮 **Konami Code Easter Egg** - Try it: ↑↑↓↓←→←→BA

### Design

- 🎨 **Spider-Man Color Scheme** - Red (#e23636) and black theme
- 🔤 **Custom Typography** - Bangers, Orbitron, and Montserrat fonts
- 🌐 **Modern UI/UX** - Clean, professional design with personality
- 💻 **Terminal-Style Code Display** - Syntax-highlighted "About" section
- 🎯 **Hover Effects** - Interactive cards and buttons

## 🚀 Quick Start

### Option 1: Open Directly

Simply open `index.html` in your web browser:

```bash
open index.html
```

### Option 2: Local Server (Recommended)

Using Python:

```bash
python3 -m http.server 8000
```

Then visit: `http://localhost:8000`

Using Node.js (with http-server):

```bash
npx http-server -p 8000
```

## 📁 Project Structure

```
Personal-Portfolio-wd-/
├── index.html           # Main HTML file
├── style.css            # All styles and animations
├── script.js            # JavaScript functionality
├── assets/
│   ├── favicon.svg      # Spider symbol favicon
│   └── Gaurav_Resume.pdf # Resume download
└── README.md            # This file
```

## 🛠️ Customization Guide

### 1. Personal Information

**In `index.html`:**

- **Line 6**: Change the page title
- **Line 7**: Update meta description
- **Line 54**: Change your name in the logo
- **Line 78**: Update your name in hero title
- **Line 118**: Edit your bio/description
- **Line 120**: Update education and experience
- **Line 126-129**: Add your tech stack icons

**Social Links (Line 103-111):**

```html
<a href="YOUR_GITHUB_URL" ...>
  <a href="YOUR_LINKEDIN_URL" ...> <a href="mailto:YOUR_EMAIL" ...></a></a
></a>
```

**Contact Info (Lines 345-357):**

```html
<a href="mailto:YOUR_EMAIL">YOUR_EMAIL</a>
<a href="YOUR_LINKEDIN_URL">YOUR_LINKEDIN</a>
<a href="YOUR_GITHUB_URL">YOUR_GITHUB</a>
```

### 2. Projects/Missions

Replace the placeholder projects (starting Line 256) with your own:

```html
<div class="mission-card" data-tilt>
  <div class="mission-image">
    <img src="path/to/your/project-image.jpg" alt="Project Name" />
    <div class="mission-overlay">
      <a href="LIVE_DEMO_URL" class="mission-link" target="_blank">
        <i class="fas fa-external-link-alt"></i>
      </a>
      <a href="GITHUB_REPO_URL" class="mission-link" target="_blank">
        <i class="fab fa-github"></i>
      </a>
    </div>
  </div>
  <div class="mission-content">
    <span class="mission-category">Project Type</span>
    <h3>Project Name</h3>
    <p>Project description goes here...</p>
    <div class="mission-tech">
      <span>Tech1</span>
      <span>Tech2</span>
      <span>Tech3</span>
    </div>
  </div>
</div>
```

### 3. Skills/Powers

Edit the skills section (starting Line 150) to match your expertise:

```html
<div class="power-card" data-tilt>
  <div class="power-icon">
    <i class="fab fa-your-icon"></i>
  </div>
  <h3>Your Skill Category</h3>
  <div class="power-tech">
    <span class="tech-tag">Technology 1</span>
    <span class="tech-tag">Technology 2</span>
  </div>
  <div class="power-bar">
    <div class="power-fill" data-power="85"></div>
    <!-- 0-100 -->
  </div>
</div>
```

### 4. Stats Numbers

Update the stats (Lines 140-150):

```html
<div class="stat-number" data-target="YOUR_NUMBER">0</div>
<div class="stat-label">Your Label</div>
```

### 5. Profile Photo

Replace the placeholder image (Line 102) with your actual photo:

```html
<img src="assets/profile-photo.jpg" alt="Gaurav" />
```

### 6. Resume

Replace `assets/Gaurav_Resume.pdf` with your actual resume PDF.

### 7. Colors

To change the color scheme, edit CSS variables in `style.css` (Lines 1-10):

```css
:root {
  --primary-red: #e23636; /* Main accent color */
  --dark-red: #b91c1c; /* Darker accent */
  --black: #000000; /* Background */
  --white: #ffffff; /* Text */
}
```

### 8. Typed Text Animation

Edit the typing animation in `script.js` (Lines 65-75):

```javascript
strings: [
    'Your Role 1',
    'Your Role 2',
    'Your Role 3'
],
```

## 📧 Email Integration

To make the contact form functional, integrate with EmailJS:

1. Sign up at [EmailJS](https://www.emailjs.com/)
2. Create an email service and template
3. In `script.js` (Line 343), uncomment and configure:

```javascript
// Initialize EmailJS
emailjs.init("YOUR_PUBLIC_KEY");

// In the form submit handler:
emailjs
  .send("YOUR_SERVICE_ID", "YOUR_TEMPLATE_ID", formData)
  .then(() => {
    // Success
  })
  .catch((error) => {
    // Error
  });
```

## 🎨 Icons

Icons are from Font Awesome. Browse available icons at [fontawesome.com](https://fontawesome.com/icons)

Change any icon by updating the class:

```html
<i class="fab fa-react"></i>
<!-- React icon -->
<i class="fas fa-code"></i>
<!-- Code icon -->
<i class="fab fa-node-js"></i>
<!-- Node.js icon -->
```

## 📱 Responsive Breakpoints

The design adapts at these breakpoints:

- **Desktop**: > 968px
- **Tablet**: 640px - 968px
- **Mobile**: < 640px

## 🎭 Libraries Used

- **[Particles.js](https://github.com/VincentGarreau/particles.js/)** - Particle background
- **[Vanilla Tilt.js](https://micku7zu.github.io/vanilla-tilt.js/)** - 3D tilt effect
- **[Typed.js](https://github.com/mattboldt/typed.js/)** - Typing animation
- **[Font Awesome](https://fontawesome.com/)** - Icons
- **[Google Fonts](https://fonts.google.com/)** - Typography

## 🎮 Easter Eggs

Try the Konami Code: Press `↑` `↑` `↓` `↓` `←` `→` `←` `→` `B` `A` on your keyboard!

## 🚀 Performance Tips

1. **Optimize Images**: Compress project images before uploading
2. **Lazy Loading**: Images already use `loading="lazy"`
3. **Minify**: Minify CSS/JS for production
4. **CDN**: Libraries are loaded from CDN for faster delivery

## 📄 Browser Support

- ✅ Chrome (recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ⚠️ IE11 (limited support)

## 🐛 Troubleshooting

**Animations not working?**

- Make sure JavaScript is enabled
- Check browser console for errors
- Ensure all CDN libraries are loading

**Tilt effect not working?**

- Vanilla Tilt requires the element to have `data-tilt` attribute
- Check that the library loaded from CDN

**Particles not showing?**

- Verify particles.js is loaded
- Check console for initialization errors

## 📝 License

This project is open source and free to use. Feel free to customize it for your own portfolio!

## 🤝 Credits

**Design Inspiration**: Spider-Man, Marvel, Spider-Verse  
**Developer**: Gaurav  
**Theme**: "With great code comes great responsibility"

---

## 🎯 Next Steps

1. ✅ Replace all placeholder content with your information
2. ✅ Add real project images and links
3. ✅ Upload your actual resume PDF
4. ✅ Set up EmailJS for contact form
5. ✅ Add your profile photo
6. ✅ Test on multiple devices
7. ✅ Deploy to hosting (Vercel, Netlify, GitHub Pages)

## 🌐 Deployment

### GitHub Pages

```bash
git add .
git commit -m "Initial Spider-Man portfolio"
git push origin main
```

Then enable GitHub Pages in repository settings.

### Vercel

```bash
npm i -g vercel
vercel
```

### Netlify

Drag and drop the folder to [app.netlify.com](https://app.netlify.com/)

---

**Built with 🕷️ and ❤️**

_"Anyone can wear the mask. You can wear the mask."_
