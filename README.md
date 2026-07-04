# Md Shamiul Islam — Portfolio

A modern, responsive personal portfolio website built with pure HTML, CSS, and JavaScript. No build step, no dependencies — deploys directly to **GitHub Pages**.

**Live site:** [shamiul110107.github.io](https://shamiul110107.github.io)

---

## Features

- Dark theme with purple/teal accent palette and CSS custom properties
- Typing hero cycling through professional titles
- Scroll-reveal animations via `IntersectionObserver`
- Animated counters (9+ years, 50M+ downloads, 80%+ test coverage)
- Sticky navbar with active section highlighting and mobile hamburger menu
- Timeline layout for experience and education
- Project cards with App Store links and image overlays
- Certification cards linking to credential pages
- Resume download section
- Password-gated year review page (SHA-256 via Web Crypto API)
- Reunion photo-frame micro-app (Bengali UI, fully client-side)

---

## Pages

| Route | Description |
|---|---|
| `/` | Main portfolio — hero, about, skills, experience, education, certifications, projects, resume, contact |
| `/ai-workflow.html` | AI-assisted iOS development workflow (Cursor, Claude, ChatGPT, MCP) |
| `/recent-learning.html` | In-progress learning topics (design principles, React Native, Snowflake) |
| `/year-review.html` | Private 2025 year review behind a SHA-256 password gate |
| `/reunion/` | Haripur High School reunion photo-frame tool |

---

## Tech Stack

| Category | Details |
|---|---|
| Markup | HTML5 |
| Styling | Vanilla CSS3 — custom properties, flexbox/grid, media queries |
| Scripting | Vanilla JavaScript (ES6+) |
| Fonts | Google Fonts — Inter (300–800) |
| Icons | Font Awesome 6.5.1 via CDN |
| Privacy | Web Crypto API (`crypto.subtle.digest` SHA-256) for year review gate |
| Storage | `sessionStorage` for year review unlock state |
| Hosting | GitHub Pages (static file serving, no server) |

---

## Project Structure

```
portfolio/
├── index.html              # Main portfolio (entry point)
├── style.css               # Shared design system & main page styles
├── script.js               # Typing effect, scroll-reveal, counters, nav
├── resume.pdf              # Downloadable resume
│
├── ai-workflow.html        # AI workflow page
├── ai-workflow.css
│
├── recent-learning.html    # Current learning topics
├── recent-learning.css
│
├── year-review.html        # Password-gated 2025 year review
├── year-review.css
│
├── images/                 # Project screenshot thumbnails
│   ├── aircloud.jpg
│   ├── central.jpg
│   ├── infiniti.jpg
│   ├── major-cineplex.jpg
│   ├── mygp.jpg
│   └── nissan.jpg
│
└── reunion/                # Standalone Bengali photo-frame tool
    ├── index.html
    ├── reunion.css
    └── frame.png
```

---

## Getting Started

No installation or build step required.

```bash
# Clone the repo
git clone https://github.com/shamiul110107/shamiul110107.github.io.git
cd shamiul110107.github.io

# Run locally with Python
python3 -m http.server 8000
# Open http://localhost:8000
```

---

## Customization

All content lives in `index.html`. Key things to update:

| What | Where |
|---|---|
| Name, initials logo (`SI.`) | `index.html` — nav logo and hero |
| Typing titles | `titles` array in `script.js` |
| About stats | `index.html` `#about` section |
| Skills | `index.html` `#skills` section |
| Experience / Education | `index.html` timeline items |
| Projects + App Store links | `index.html` `#projects` section + `images/` folder |
| Certifications | `index.html` `#certifications` section |
| Social links (email, phone, LinkedIn, GitHub) | `index.html` `#contact` section and footer |
| Resume | Replace `resume.pdf` in the project root |
| Accent colors | CSS variables `--primary` and `--accent` in `style.css` `:root` |

> **Note:** The contact section uses direct mailto/tel/social links. There is no contact form.

---

## Deployment

```bash
git add .
git commit -m "Update portfolio"
git push -u origin main
```

Then go to **Settings → Pages** in your GitHub repository and set the source to the `main` branch. Your site will be live at `https://<username>.github.io`.

---

## Security Note (Year Review)

The year review page (`year-review.html`) is protected by a client-side SHA-256 password check. This is obfuscation only — the content is visible in the HTML source. Do not use this pattern for genuinely sensitive data.

---

## License

MIT — free to use and customize.

---

## Author

**Md Shamiul Islam** — Senior Mobile / iOS Developer, Bangkok  
[GitHub](https://github.com/shamiul110107) · [LinkedIn](https://linkedin.com/in/shamiul110107) · shamiulcse.pust@gmail.com
