# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static landing page for UC APEX Upgrades, a comprehensive Oracle APEX modernization service. The site is built using vanilla HTML5, CSS3, and JavaScript with no build system or dependencies.

## Architecture

### File Structure
```
/
├── index.html              # Main landing page with all sections
├── styles/main.css         # Complete stylesheet with CSS variables
├── scripts/main.js         # Interactive functionality and animations
├── assets/                 # Static assets
│   └── united-codes-logo.svg
└── README.md              # Basic project description
```

### Key Components

**HTML Structure (`index.html`):**
- Single-page application with semantic HTML5 sections
- Responsive navigation with mobile menu
- Progressive form with comprehensive validation
- Accessibility-first markup with proper ARIA labels
- Contact form for lead generation (`#assessmentForm`)

**Styling (`styles/main.css`):**
- CSS custom properties (variables) for consistent theming
- Mobile-first responsive design approach
- Modular component-based styling
- Smooth animations and transitions
- Brand colors: Primary blue (`#4a5d8a`), Secondary (`#6b7ba8`), Accent (`#2c3e50`)

**JavaScript (`scripts/main.js`):**
- Vanilla JavaScript with no external dependencies
- Modular function-based architecture with init pattern
- Key modules: smooth scrolling, scroll animations, mobile menu, form validation
- Intersection Observer API for performance-optimized animations
- Progressive enhancement approach

## Development Workflow

### Local Development
- No build process required - serve files directly
- Use any static file server (e.g., `python -m http.server`, Live Server extension)
- All changes are immediate - no compilation step needed

### Code Style
- Use CSS custom properties for consistent theming
- Follow semantic HTML5 structure
- Maintain mobile-first responsive design
- Use modern JavaScript (ES6+) features
- Implement progressive enhancement principles

### Form Handling
- Contact form (`#assessmentForm`) currently simulates submission
- Form validation is client-side with real-time feedback
- Replace simulation logic in `scripts/main.js:149-169` with actual backend integration

## Key Features

### Interactive Elements
- Smooth scroll navigation with offset calculation
- Intersection Observer-based scroll animations
- Mobile hamburger menu with CSS transitions
- Form validation with real-time error display
- Notification system for user feedback

### Performance Optimizations
- Lazy-loaded animations triggered by scroll
- Staggered card animations for visual appeal
- Debounced scroll events
- Service Worker ready (commented implementation)

### Analytics Integration
- GTM/Google Analytics event tracking placeholders
- CTA click tracking implemented
- Conversion tracking ready for implementation

## Making Changes

### Styling Changes
- All colors defined in CSS custom properties at `:root`
- Component styles are modular and clearly separated
- Responsive breakpoints follow mobile-first approach

### Content Updates
- All content is inline in `index.html` for easy editing
- Section structure is semantic and well-commented
- Form fields and options easily configurable

### Adding Functionality
- Follow existing modular pattern in `main.js`
- Initialize new functions in `DOMContentLoaded` event handler
- Use existing utility functions (`debounce`, error handling)

## Browser Support
- Modern browsers with ES6+ support
- Fallbacks provided for older browsers (smooth scroll polyfill)
- Progressive enhancement ensures basic functionality always works