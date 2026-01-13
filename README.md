# YogaLife - Static HTML Website

This folder contains a complete static HTML, CSS, and JavaScript version of the YogaLife yoga website.

## File Structure

```
static/
├── index.html          # Home page with all sections
├── about.html          # About Us page
├── contact.html        # Contact Us page with form
├── privacy.html        # Privacy Policy page
├── terms.html          # Terms & Conditions page
├── styles.css          # All CSS styles
├── script.js           # All JavaScript functionality
└── README.md           # This file
```

## Features

### Home Page (index.html)
- **Fixed Header**: Sticky navigation with mobile menu
- **Hero Slider**: Auto-rotating image slider with 3 slides
  - Manual navigation with arrow buttons
  - Dot indicators
  - Auto-advance every 5 seconds
- **Yoga Asanas Section**: 6-card grid with yoga poses
- **Numbers Speak Section**: Animated counters (triggers on scroll)
- **Benefits Section**: Image with bullet-point list
- **Testimonials**: Carousel with 3 client testimonials
- **Footer**: Multi-column footer with links

### Other Pages
- **About Us**: Company story and values
- **Contact Us**: Contact information and working form
- **Privacy Policy**: Full privacy policy content
- **Terms & Conditions**: Complete terms and conditions

## JavaScript Functionality

All interactive features are implemented in `script.js`:

1. **Mobile Menu Toggle**
   - Hamburger menu for mobile devices
   - Smooth open/close transitions

2. **Hero Slider**
   - Auto-rotation every 5 seconds
   - Previous/Next button navigation
   - Dot indicator navigation
   - Smooth fade transitions

3. **Animated Counters**
   - Counts up from 0 to target number
   - Triggers when section scrolls into view
   - Only animates once per page load

4. **Testimonial Carousel**
   - Manual navigation with arrows
   - Dot indicators for position
   - Smooth transitions

5. **Contact Form**
   - Form validation
   - Success message on submission
   - Form reset after submission

6. **Smooth Scrolling**
   - All anchor links scroll smoothly

## Styling

The website uses a calm, peaceful color scheme:
- **Primary Green**: `#059669` (Emerald)
- **Dark Green**: `#064e3b`
- **Light Green**: `#d1fae5`
- **Text Colors**: Gray scale from `#374151` to `#6b7280`
- **White Background**: `#ffffff`

### Responsive Design
- Mobile-first approach
- Breakpoints:
  - Mobile: < 768px
  - Tablet: 768px - 1023px
  - Desktop: 1024px+

## How to Use

1. **Open the website**: Simply open `index.html` in a web browser
2. **Navigate**: Click on navigation links to visit different pages
3. **All pages work offline**: No external dependencies required (except images from Unsplash)

## Browser Compatibility

Works in all modern browsers:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Opera (latest)

## Customization

### Change Colors
Edit the CSS variables in `styles.css`:
- Search for color values like `#059669` and replace with your brand colors

### Change Content
- Edit the HTML files directly
- Update text, images, and links as needed

### Change Images
- Replace image URLs in HTML files
- Use local images by adding them to the folder and updating the `src` attributes

### Adjust Timing
In `script.js`:
- Slider speed: Change `5000` (5 seconds) in the `setInterval` function
- Counter animation: Change `2000` (2 seconds) in the `duration` variable

## Notes

- All images are loaded from Unsplash CDN
- For production use, download images locally for better performance
- Contact form currently shows an alert - integrate with a backend service for real functionality
- Smooth scroll behavior works in all modern browsers

## Converting Back to React

If you need to convert back to React:
1. Each HTML file represents a page component
2. Sections in index.html can be split into separate components
3. JavaScript functions can be converted to React hooks (useState, useEffect)
4. CSS can be used as-is or converted to CSS modules

---

Built with ❤️ for YogaLife
