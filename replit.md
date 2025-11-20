# BizCraft Studio - Corporate Website

## Overview
BizCraft Studio is a fictional corporate website for a production studio specializing in bespoke business systems, websites, and AI tools for small to medium-sized businesses and sole proprietors. The project aims to showcase a "business x craft" approach to development, offering tailored solutions to clients. The business vision is to provide high-quality, customized digital solutions, focusing on AI/SaaS aesthetics and modern technology to build trust and demonstrate craftsmanship.

## User Preferences
I prefer detailed explanations.
I want iterative development.
Ask before making major changes.

## System Architecture

### UI/UX Decisions
The design adopts a dark, technology-themed aesthetic, inspired by AI/SaaS interfaces (e.g., aidealab.com).
- **Color Scheme**: Primarily dark blue/black (`#0A0E27`, `#0F172A`, `#1E293B`) with cyan/light blue accents (`#00D9FF`, `#38BDF8`). Text is white/light gray.
- **Visual Elements**: Features include data visualization-style background images (blue swirl in hero), floating circular elements with radial gradients, gradient borders, emoji icons for visual cues, and 3D spherical elements in the hero section.
- **Interactivity**: Extensive CSS animations (fadeInUp, float, pulse, shimmer), hover effects with transitions, and multi-layered shadow designs are used.
- **Responsiveness**: Fully responsive across PC, tablet, and mobile, with a mobile-first approach.

### Technical Implementations
- **Technology Stack**: Pure HTML5 and CSS3. No JavaScript is used for any interactive elements, including a CSS-only hamburger menu implemented via checkbox + label hack.
- **CSS Architecture**: Organized with a BEM-like naming convention (e.g., `.header`, `.card__title`). Includes sections for reset/base styles, animations, layout, header/navigation, components, forms, and media queries.
- **CSS Features**: Utilizes Flexbox and Grid for layout, `@keyframes` for animations, and CSS pseudo-elements (`::before`, `::after`) for iconography and decorative elements. Gradient effects are extensively used on backgrounds, buttons, and icons.

### Feature Specifications
- **Core Pages**: `index.html` (hero, reasons, services), `service-system.html`, `service-website.html`, `service-ai.html` (detailed service pages), `works.html` (portfolio), `voice.html` (testimonials), `price.html`, `about.html`, `contact.html`.
- **Service Flow**: Simplified 4-step process for System/Website development and a 3-step process for AI tool development.
- **Dynamic Elements**: Reasons section expanded to 5 items with AI-generated images and responsive layouts. Service section redesigned with AI-generated holographic interface-style images and responsive grid.
- **CTA**: A prominent Call-to-Action section is included between the service section and footer.
- **Navigation**: Comprehensive navigation linking to all main sections and detailed service pages.

### System Design Choices
- **Static Site**: Implemented as a static HTML site, intended for future migration to a WordPress theme, thus maintaining a simple and dependency-free structure.
- **File Structure**: Organized with a dedicated `style.css` for global styles and individual HTML files for each page.
- **Accessibility**: Semantic HTML5 tags are used throughout the structure.

## External Dependencies
None. The project is built using pure HTML and CSS with no external libraries, frameworks, or third-party services integrated.