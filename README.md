# 🚀 Saravanan — Full-Stack Developer Portfolio

Welcome to the repository for my professional portfolio! I built this project to showcase my work as a **Full-Stack Developer**, integrating modern web technologies with a focus on high-performance UI and interactive user experiences.

---

## 🛠️ How This Portfolio Was Built

This project is a **modern, single-page application (SPA)** designed for speed, clean code architecture, and a premium "glassmorphism" aesthetic.

### 1. The Core Stack
*   **HTML5 & Semantic Structure:** Designed for SEO and accessibility, using meta tags for Open Graph sharing and clear ARIA labels.
*   **Tailwind CSS:** Used for rapid, responsive UI development. Features a custom configuration for typography (*PT Sans* and *DM Sans*) and a vibrant **Accent Orange (#FF6B2B)** color palette.
*   **Alpine.js:** A lightweight framework used to handle site state, including the dark mode toggle, mobile menu transitions, and active scroll tracking.

### 2. Custom Visual Engineering
I implemented several advanced CSS and SVG techniques to give the site a premium feel:
*   **Fractal Noise Overlay:** A custom SVG filter applied to the body to create a subtle, high-end texture.
*   **Glassmorphism Header:** Uses `backdrop-blur-md` and semi-transparent backgrounds to remain stylish and visible while scrolling.
*   **Custom Scrollbar:** A themed scrollbar that matches the portfolio’s accent colors for a cohesive brand experience.

---

## 🎨 Interactive Animations & Code

Below are the technical implementations that power the portfolio's interactivity:

### ✨ Shimmer Button Effect
Used on "Hire Me" and "See Projects" buttons to draw user attention with a sleek light-streak animation.

```css
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
