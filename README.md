# Portfolio Website

A modern, responsive personal portfolio website showcasing your projects, skills, and contact information.

## 🚀 Features

- **Responsive Design** - Works perfectly on all devices (desktop, tablet, mobile)
- **Modern UI/UX** - Clean and professional design with smooth animations
- **Interactive Elements** - Animated skill bars, smooth scrolling, and hover effects
- **Contact Form** - Functional contact form for visitors to reach you
- **Easy Customization** - Well-organized code structure for easy modifications
- **Fast Loading** - Optimized for performance with lazy loading
- **SEO Friendly** - Proper HTML structure and meta tags

## 📁 Project Structure

```
portfolio-website/
│
├── index.html          # Main HTML file
├── css/
│   └── style.css       # All styles
├── js/
│   └── script.js       # Interactive functionality
├── assets/
│   ├── images/         # Your images
│   └── resume.pdf      # Your resume (optional)
└── README.md           # This file
```

## 🛠️ Customization Guide

### 1. Personal Information

Open `index.html` and update:

- **Line 35**: Your name in the hero section
- **Line 36**: Your title/subtitle
- **Line 37**: Your description
- **Lines 44-56**: Social media links
- **Lines 79-90**: About section content
- **Line 370**: Footer copyright text

### 2. Skills

Update the skills section (Lines 110-180 in `index.html`):
- Modify skill categories
- Adjust skill progress bars (change `style="width: XX%"`)
- Add or remove skills as needed

### 3. Projects

Edit project cards (Lines 195-285):
- Update project titles and descriptions
- Change project tags
- Add your GitHub and demo links
- Replace icon classes with appropriate Font Awesome icons

### 4. Contact Information

Update contact details (Lines 305-318):
- Email address
- Phone number
- Location
- Social links

### 5. Colors & Theme

Customize the color scheme in `css/style.css` (Lines 1-12):

```css
:root {
    --primary-color: #6366f1;      /* Main brand color */
    --secondary-color: #8b5cf6;    /* Secondary accent */
    --accent-color: #ec4899;       /* Highlight color */
    /* ... other variables */
}
```

### 6. Images

Replace the placeholder profile image:
1. Add your photo to `assets/images/`
2. Update line 95 in `index.html`:
   ```html
   <img src="assets/images/your-photo.jpg" alt="Your Name">
   ```

## 🚀 Getting Started

### Quick Start

1. **Download/Clone** this repository
2. **Customize** the content (see guide above)
3. **Add your images** to the `assets/images/` folder
4. **Open** `index.html` in your browser

### Local Development

Simply open `index.html` in any modern web browser. No build process required!

### Using Live Server (Recommended)

If you're using VS Code:

1. Install the "Live Server" extension
2. Right-click on `index.html`
3. Select "Open with Live Server"
4. Your site will open at `http://localhost:5500`

## 📤 Deployment Options

### Option 1: GitHub Pages (Free)

1. Create a GitHub repository
2. Push your code
3. Go to Settings → Pages
4. Select branch and save
5. Your site will be live at `https://yourusername.github.io/repository-name`

### Option 2: Netlify (Free)

1. Create a Netlify account
2. Drag and drop your project folder
3. Get instant deployment with custom domain support

### Option 3: Vercel (Free)

1. Sign up at vercel.com
2. Import your GitHub repository
3. Deploy with one click

### Option 4: Traditional Hosting

Upload all files to your web hosting via FTP/SFTP.

## 🎨 Adding Your Resume

1. Save your resume as `resume.pdf`
2. Place it in the `assets/` folder
3. The download button is already linked (line 93)

## 📧 Contact Form Setup

The current form shows a demo alert. To make it functional:

### Option 1: FormSpree (Easiest)

1. Sign up at [formspree.io](https://formspree.io)
2. Get your form endpoint
3. Update form action in `index.html`:
   ```html
   <form action="https://formspree.io/f/YOUR_ID" method="POST">
   ```

### Option 2: EmailJS

1. Sign up at [emailjs.com](https://www.emailjs.com/)
2. Follow their integration guide
3. Update the form submission code in `js/script.js`

### Option 3: Custom Backend

Uncomment the fetch code in `js/script.js` (lines 174-190) and point it to your API.

## 🎯 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## 📱 Mobile Optimization

The site is fully responsive with:
- Mobile-friendly navigation (hamburger menu)
- Touch-optimized buttons
- Responsive grid layouts
- Optimized images

## 🔧 Tech Stack

- **HTML5** - Semantic markup
- **CSS3** - Modern styling with CSS Grid & Flexbox
- **Vanilla JavaScript** - No dependencies, pure JS
- **Font Awesome 6** - Icons (CDN)

## 📈 Performance Tips

1. **Optimize images**: Use WebP format and compress images
2. **Lazy loading**: Images load only when needed (already implemented)
3. **Minify files**: Before deployment, minify CSS and JS
4. **Enable caching**: Configure proper cache headers on your server

## 🎓 Learning Resources

If you want to learn more about the technologies used:
- [MDN Web Docs](https://developer.mozilla.org/) - HTML, CSS, JavaScript
- [CSS-Tricks](https://css-tricks.com/) - Modern CSS techniques
- [JavaScript.info](https://javascript.info/) - JavaScript tutorials

## 🐛 Troubleshooting

### Icons not showing?
- Check your internet connection (Font Awesome loads from CDN)
- Or download Font Awesome locally

### Form not working?
- Implement one of the contact form options above
- Check browser console for errors

### Styling issues?
- Clear browser cache
- Check that `css/style.css` path is correct
- Verify all files are in correct folders

## 💡 Customization Ideas

- Add a blog section
- Include testimonials
- Add a dark/light theme toggle
- Implement project filters
- Add more animations
- Create a timeline for experience
- Add certifications section
- Include a skills progress animation

## 📝 License

This project is open source and available for personal and commercial use.

## 🤝 Contributing

Feel free to fork this project and customize it for your needs!

## 📞 Support

If you need help customizing this portfolio:
- Check the HTML comments for guidance
- Review this README carefully
- Google is your friend for specific CSS/JS questions

## 🌟 Show Your Support

If you found this helpful:
- ⭐ Star the repository
- 🍴 Fork it for your own use
- 📢 Share it with others

---

**Built with ❤️ for developers by developers**

Good luck with your portfolio! 🚀
