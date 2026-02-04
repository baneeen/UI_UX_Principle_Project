# Alex Styles - Portfolio Website

A modern, responsive portfolio website showcasing UI/UX design work with interactive components, smooth animations, and accessible design practices.

## 🎨 Features

### Interactive Components
- **Buttons** - 6 hover effect variants (Primary, Outline, Ghost, 3D, Neon, Underline)
- **Modal Dialog** - Accessible project detail viewer with focus trapping and keyboard controls
- **Tooltips** - Navigation tooltips with positioning and keyboard support
- **Animations** - Smooth entrance effects and interactive transitions

### Design System
- **Design Tokens** - Centralized CSS custom properties for consistent theming
- **Modular Typography Scale** - 1.2x scale for harmonious sizing
- **Color Palette** - Cyan primary, slate secondary, amber accent
- **Responsive Grid** - CSS Grid and Flexbox layouts
- **Shadow System** - 5 shadow levels for depth

### Responsive Design
- Mobile-first approach
- Breakpoints: 768px (mobile), 1024px (tablet), 1025px+ (desktop)
- Optimized layouts for all screen sizes
- Touch-friendly interactive elements

### Accessibility
- Semantic HTML5 structure
- ARIA labels and roles for modals and dialogs
- Keyboard navigation support (Tab, Escape)
- Focus trapping in modal
- Sufficient color contrast
- Readable typography with comfortable measure (65ch max-width)

## 📁 File Structure

```
├── index.html           # Main portfolio page
├── styles.css          # Organized stylesheet (1029 lines)
├── buttons.html        # Standalone button demo
└── README.md           # This file
```

## 🚀 Getting Started

### View the Portfolio
1. Open `index.html` in your web browser
2. Click on navigation links to scroll to sections
3. Hover over navigation items to see tooltips
4. Click on project cards to view details in the modal

### View Button Styles
Open `buttons.html` to see all 6 button hover effects with the dark theme.

## 🎯 CSS Architecture

### Organization
The stylesheet is organized into logical sections for maintainability:

1. **Design Tokens** (lines 5-115)
   - Typography scale, weights, line heights
   - Color palette with tints and shades
   - Spacing scale, shadows, gradients

2. **Animations** (lines 116-140)
   - FadeInUp, FadeIn, SlideInLeft, SlideInRight, ScaleIn

3. **Base Styles** (lines 142-203)
   - CSS reset, responsive html sizing
   - Body typography and rendering

4. **Typography Utilities** (lines 168-202)
   - Prose width, heading styles
   - Comfortable text measure

5. **Layout System** (lines 204-244)
   - Container utilities
   - Section and main grid flex

6. **Header & Navigation** (lines 245-322)
   - Gradient header with shadow
   - Sticky navigation with underline hover effect

7. **About Section** (lines 323-429)
   - Two-column grid layout
   - Skills tags with hover scale effect

8. **Portfolio Section** (lines 430-555)
   - Auto-fit grid with project cards
   - Card hover effects with lift animation
   - Project link styling

9. **Contact Section** (lines 556-684)
   - Centered form layout
   - Styled inputs with focus states
   - Gradient submit button

10. **Footer** (lines 685-699)
    - Dark background footer

11. **Buttons** (lines 702-828)
    - Base button styles and focus states
    - 6 button variants with different hover effects

12. **Modal & Overlay** (lines 831-978)
    - Fixed overlay with semi-transparent backdrop
    - Animated modal with scale and opacity
    - Accessible close button

13. **Tooltips** (lines 981-1010)
    - Positioned tooltips with arrow
    - Scale and fade animation

14. **Responsive Design** (lines 703-830)
    - Mobile adjustments (max-width: 768px)
    - Tablet optimizations (max-width: 1024px)
    - Desktop enhancements (min-width: 1025px)

### Key CSS Practices
- ✅ CSS custom properties for theming
- ✅ Mobile-first responsive design
- ✅ CSS Grid for layouts
- ✅ Flexbox for alignment
- ✅ Cubic-bezier easing for smooth animations
- ✅ Clamp() for responsive typography
- ✅ No external dependencies (except Google Fonts)

## 🎨 Customization Guide

### Change Brand Colors
Edit the color variables in `:root` (lines 41-60):
```css
--color-primary: #06b6d4;        /* Change primary color */
--color-secondary: #334155;      /* Change secondary color */
--color-accent: #f59e0b;         /* Change accent color */
```

### Adjust Typography Scale
Modify font size variables (lines 18-27):
```css
--fs-base: 1rem;     /* Base size */
--fs-md: 1.2rem;     /* Multiplier: 1.2x */
```

### Change Spacing
Update spacing tokens (lines 105-112):
```css
--space-sm: 12px;
--space-md: 18px;
--space-lg: 28px;
```

### Modify Animations
Adjust animation timing in @keyframes (lines 117-140) or transition durations in component styles.

### Customize Breakpoints
Change responsive breakpoints in media queries (lines 703-830):
```css
@media (max-width: 768px)   /* Mobile */
@media (max-width: 1024px)  /* Tablet */
@media (min-width: 1025px)  /* Desktop */
```

## 🌐 Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

### Features Used
- CSS Grid
- CSS Flexbox
- CSS Custom Properties
- CSS Gradients
- CSS Animations
- CSS Transforms
- Media Queries
- Clamp() function

## ⌨️ Keyboard Navigation

- **Tab** - Navigate through interactive elements
- **Enter/Space** - Activate buttons and open modal
- **Escape** - Close modal

## 📋 Content Sections

### Header
- Portfolio title "Alex"
- Subtitle with profession

### Navigation
- About Me (with tooltip)
- Portfolio (with tooltip)
- Contact (with tooltip)

### About Section
- Profile description
- Skills tags
- Contact call-to-action

### Portfolio Section
- 6 project cards with:
  - Project thumbnail with gradient
  - Project title and description
  - Interactive "Learn More" link (opens modal)

### Contact Section
- Contact form with fields:
  - Name
  - Email
  - Message
  - Submit button

### Footer
- Copyright information

## 🔧 JavaScript Features

### Modal Manager
- Opens on project card click
- Prevents body scroll
- Traps focus within modal
- Closes on Escape key or close button

### Tooltip Manager
- Shows on hover and focus
- Positions above navigation links
- Arrow points to trigger element
- Respects reduced motion preferences

## 📊 Performance

- No external libraries or frameworks
- Lightweight CSS (~30KB minified potential)
- Optimized animations (GPU-accelerated)
- Responsive images ready
- Font optimization via Google Fonts

## 📄 License

MIT License

Copyright (c) 2026 Alex Styles

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## 🎓 Learning Resources

This project demonstrates:
- CSS Grid layouts for responsiveness
- Flexbox for component alignment
- CSS custom properties for maintainability
- Animation techniques with @keyframes
- Accessibility best practices
- Semantic HTML structure
- Mobile-first design approach
- Component-based CSS organization

## 📞 Support

For modifications or questions about the design system, refer to the organized CSS sections. Each section is clearly commented with its purpose and scope.

---

**Built with HTML5, CSS3, and Vanilla JavaScript**  
*No frameworks or libraries required*
