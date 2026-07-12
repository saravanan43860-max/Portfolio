🚀 Saravanan — Full-Stack Developer Portfolio
This repository contains the source code for my professional portfolio. I built this project to showcase my work as a Full-Stack Developer, integrating modern web technologies with a focus on high-performance UI and interactive user experiences
.
🛠️ How This Portfolio Was Built
The portfolio is designed as a modern, single-page application (SPA) that prioritizes speed, clean code architecture, and a "glassmorphism" aesthetic
.
1. The Core Stack
HTML5 & Semantic Structure: Designed for SEO and accessibility, using meta tags for Open Graph (social sharing) and clear ARIA labels for navigation
.
Tailwind CSS (Utility-First Styling): Used for rapid, responsive UI development. I implemented a custom configuration for typography (PT Sans and DM Sans) and a specific color palette featuring a vibrant Accent Orange (#FF6B2B)
.
Alpine.js (Lightweight Reactivity): Instead of a heavy framework, I used Alpine.js to handle the site's state, such as the dark mode toggle, mobile menu transitions, and active scroll tracking
.
2. Custom Visual Engineering
I implemented several advanced CSS and SVG techniques to give the site a premium feel:
Fractal Noise Overlay: A custom SVG filter is applied to the body to create a subtle, high-end texture
.
Glassmorphism Header: The navigation bar uses backdrop-blur-md and semi-transparent backgrounds to remain visible while scrolling
.
Custom Scrollbar: A themed scrollbar that matches the portfolio’s accent colors for a cohesive brand experience
.
🎨 Interactive Animations & Code
Below are the specific technical implementations that power the portfolio's interactivity.
✨ Shimmer Button Effect (CSS)
Used on "Hire Me" and "See Projects" buttons to draw user attention with a sleek light-streak animation
.
.shimmer {
  position: relative;
  overflow: hidden;
}

.shimmer::after {
  content: '';
  position: absolute;
  top: 0;
  left: -100%;
  width: 60%;
  height: 100%;
  background: rgba(255,255,255,.18);
  transform: skewX(-20deg);
  transition: left .4s cubic-bezier(.4,0,.2,1);
}

.shimmer:hover::after {
  left: 160%;
}
