# Portfolio Website

A modern, responsive personal portfolio website built with HTML, CSS, and JavaScript. Designed to be hosted on **GitHub Pages** for free.

## Features

- Dark-themed modern design with smooth animations
- Fully responsive (mobile, tablet, desktop)
- Typing effect hero section
- Scroll-reveal animations with Intersection Observer
- Animated counters for stats
- Timeline-style experience section
- Project showcase grid
- Contact form (frontend only — integrate with a service below)
- Resume download section

## Quick Start

### 1. Fork or Clone

```bash
git clone https://github.com/shamiul110107/shamiul.github.io.git
cd shamiul.github.io
```

### 2. Customize Content

Open `index.html` and replace placeholder content:

- **Your Name** — your real name
- **YN** — your initials (used as logo)
- **Hero titles** — edit the typing titles in `script.js`
- **About section** — your bio, stats, and details
- **Skills** — your actual skill set
- **Experience** — your work history
- **Projects** — your real projects with links
- **Social links** — your GitHub, LinkedIn, Twitter, email
- **Resume** — add your `resume.pdf` file to the project root

### 3. Add Your Photo

Replace the placeholder in the hero section with your actual photo:

```html
<!-- Replace the hero-image-placeholder div with: -->
<img src="your-photo.jpg" alt="Your Name" />
```

### 4. Deploy to GitHub Pages

Push your code:

```bash
git add .
git commit -m "Initial portfolio"
git push -u origin main
```

Go to **Settings → Pages** in your repository, select `main` branch as source.
Your site will be live at `https://shamiul110107.github.io`

### 5. (Optional) Contact Form Integration

The contact form is frontend-only by default. To make it functional, integrate with one of these free services:

- **[Formspree](https://formspree.io)** — Add `action="https://formspree.io/f/YOUR_ID"` and `method="POST"` to the form tag
- **[EmailJS](https://www.emailjs.com)** — Client-side email sending via JavaScript
- **[Netlify Forms](https://docs.netlify.com/forms/setup/)** — If hosting on Netlify

## Project Structure

```
portfolio/
├── index.html      # Main HTML file
├── style.css       # All styles
├── script.js       # Interactions & animations
├── resume.pdf      # Your resume (add this)
└── README.md       # This file
```

## License

MIT — feel free to use and customize.
