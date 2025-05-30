# basic-landing-page
# Responsive Web Page Conversion

This project involves converting a static, desktop-only webpage into a responsive design that adapts seamlessly across mobile, tablet, and desktop devices.

## 📱 Objective

Make the existing desktop layout mobile-friendly using **CSS media queries**, ensuring a smooth user experience on all screen sizes.

## 🛠️ Tools Used

- HTML5
- CSS3
- Media Queries
- Visual Studio Code (VS Code)
- Chrome DevTools (for responsive testing)

## 📁 Project Structure

project-root/
├── index.html
├── style.css
└── assets/
└── images/

## 🧩 Features

- Mobile-first responsive layout using `@media` queries
- Fluid typography and spacing
- Flexible grid layout for service cards
- Optimized header and navigation for smaller screens
- Adaptive container and section widths

## ⚙️ How to Use

1. Clone the repository or download the files.
2. Open `index.html` in your browser.
3. Use Chrome DevTools or any browser's device toolbar to test responsiveness.

## 🖥️ Desktop vs Mobile Behavior

| Feature             | Desktop                          | Mobile/Tablets                      |
|---------------------|----------------------------------|-------------------------------------|
| Container Width     | Fixed (`1200px`)                 | Fluid (`100%` with padding)         |
| Navigation          | Horizontal Flex Layout           | Stacked column layout               |
| Services Section    | Row layout with wrap             | Single-column vertical layout       |
| Header              | Large padding & background image | Scales down padding and font size   |
| Typography          | Large, fixed font sizes          | Relative font sizes for readability |

## ✅ Viewport Meta Tag

Make sure your HTML includes this for proper scaling on mobile:
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
@media (max-width: 768px) {
  .service-card {
    width: 80%;
  }
  nav {
    flex-direction: column;
    align-items: center;
  }
}

