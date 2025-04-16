# 🫧 Gooey Bubble Gradient Animation

A visually engaging full-screen animation of fluid, interactive "bubbles" using CSS, SVG filters, and keyframe animations.

https://user.github.io/bubbles-gradient-demo/ <!-- Replace with your GitHub Pages link if hosting -->

---

## ✨ Preview

![Preview](preview.gif) <!-- Replace with actual screenshot or GIF if available -->

---

## 🧩 Features

- SVG Gaussian Blur + Color Matrix filter for a gooey effect.
- Multiple animated radial gradients with unique movement paths.
- Customizable colors via CSS variables.
- Responsive full-page layout.
- Compatible with modern browsers.

---

## 📦 Code Overview

### HTML

```html
<div class="text-container">
  Bubbles
</div>
<div class="gradient-bg">
  <svg xmlns="http://www.w3.org/2000/svg">
    <defs>
      <filter id="goo">
        <feGaussianBlur in="SourceGraphic" stdDeviation="10" result="blur" />
        <feColorMatrix in="blur" mode="matrix"
          values="1 0 0 0 0  0 1 0 0 0  0 0 1 0 0  0 0 0 18 -8" result="goo" />
        <feBlend in="SourceGraphic" in2="goo" />
      </filter>
    </defs>
  </svg>
  <div class="gradients-container">
    <div class="g1"></div>
    <div class="g2"></div>
    <div class="g3"></div>
    <div class="g4"></div>
    <div class="g5"></div>
    <div class="interactive"></div>
  </div>
</div>

