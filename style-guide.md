# Triple A Consulting - Website Style Guide & Design System

**Version:** 1.0  
**Date:** October 2025  
**Purpose:** Complete reference for consistent design implementation

---

## 📐 BRAND COLORS

### Primary Colors
```css
--primary-blue: #1e3a8a;      /* Main brand color - Headers, CTAs */
--primary-orange: #f97316;    /* Accent color - Highlights, Links */
--primary-green: #10b981;     /* Success color - Checkmarks, Positive */
```

### Secondary Colors
```css
--blue-light: #3b82f6;        /* Gradients, Hover states */
--blue-lighter: #60a5fa;      /* Backgrounds */
--orange-light: #fb923c;      /* Gradients */
--green-light: #34d399;       /* Light success states */
```

### Neutral Colors
```css
--gray-50: #f8fafc;           /* Light backgrounds */
--gray-100: #f1f5f9;          /* Card backgrounds */
--gray-200: #e2e8f0;          /* Borders */
--gray-300: #cbd5e1;          /* Dividers */
--gray-400: #94a3b8;          /* Disabled text */
--gray-500: #64748b;          /* Secondary text */
--gray-600: #475569;          /* Body text */
--gray-700: #334155;          /* Headings */
--gray-800: #1e293b;          /* Dark text */
--gray-900: #0f172a;          /* Black text */
--white: #ffffff;             /* White */
```

### Color Usage Guidelines

**Primary Blue (#1e3a8a):**
- Navigation bar
- Main headings
- Footer background
- Primary buttons (background)
- Links (hover state)

**Primary Orange (#f97316):**
- Call-to-action buttons
- Active navigation items
- Section accents
- Icons and badges
- Links (default state)

**Primary Green (#10b981):**
- Success messages
- Checkmarks
- Form validation (success)
- Statistics/metrics

---

## 🔤 TYPOGRAPHY

### Font Families
```css
/* System Font Stack (Fast & Native) */
--font-primary: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 
                'Helvetica Neue', Arial, sans-serif;

/* Alternative: Google Fonts (if preferred) */
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap');
--font-primary: 'Inter', sans-serif;
```

### Font Sizes
```css
--text-xs: 12px;      /* Captions, labels */
--text-sm: 14px;      /* Small text, metadata */
--text-base: 16px;    /* Body text (default) */
--text-lg: 18px;      /* Large body text */
--text-xl: 20px;      /* Small headings */
--text-2xl: 24px;     /* Section subheadings */
--text-3xl: 30px;     /* Section headings (mobile) */
--text-4xl: 36px;     /* Section headings (desktop) */
--text-5xl: 48px;     /* Page headings (desktop) */
--text-6xl: 60px;     /* Hero headings (desktop) */
```

### Font Weights
```css
--font-normal: 400;   /* Body text */
--font-medium: 500;   /* Emphasized text */
--font-semibold: 600; /* Subheadings */
--font-bold: 700;     /* Headings, buttons */
```

### Line Heights
```css
--leading-tight: 1.2;   /* Headings */
--leading-snug: 1.4;    /* Subheadings */
--leading-normal: 1.6;  /* Body text */
--leading-relaxed: 1.8; /* Long-form content */
```

### Typography Scale

**Hero Heading (H1):**
```css
font-size: 48px (desktop), 32px (mobile)
font-weight: 700
line-height: 1.2
color: #1e3a8a or white
margin-bottom: 20px
```

**Page Heading (H1):**
```css
font-size: 36px (desktop), 28px (mobile)
font-weight: 700
line-height: 1.3
color: #1e3a8a
margin-bottom: 15px
```

**Section Heading (H2):**
```css
font-size: 36px (desktop), 24px (mobile)
font-weight: 700
line-height: 1.3
color: #1e3a8a
margin-bottom: 15px
```

**Subsection Heading (H3):**
```css
font-size: 24px (desktop), 20px (mobile)
font-weight: 600
line-height: 1.4
color: #1e3a8a
margin-bottom: 12px
```

**Body Text:**
```css
font-size: 16px
font-weight: 400
line-height: 1.6
color: #475569
```

---

## 📏 SPACING SYSTEM

### Spacing Scale (8px base unit)
```css
--space-1: 4px;     /* Tight spacing */
--space-2: 8px;     /* Base unit */
--space-3: 12px;    /* Small spacing */
--space-4: 16px;    /* Default spacing */
--space-5: 20px;    /* Medium spacing */
--space-6: 24px;    /* Large spacing */
--space-8: 32px;    /* Extra large */
--space-10: 40px;   /* Section padding (mobile) */
--space-12: 48px;   /* Section padding */
--space-16: 64px;   /* Section padding (desktop) */
--space-20: 80px;   /* Large section padding */
```

### Container Widths
```css
--container-sm: 640px;    /* Small content */
--container-md: 768px;    /* Medium content */
--container-lg: 1024px;   /* Large content */
--container-xl: 1200px;   /* Default max width */
--container-2xl: 1400px;  /* Wide layouts */
```

### Section Padding
```css
/* Desktop */
padding: 80px 20px;

/* Tablet */
@media (max-width: 1024px) {
  padding: 60px 20px;
}

/* Mobile */
@media (max-width: 768px) {
  padding: 40px 20px;
}
```

---

## 🎨 COMPONENT STYLES

### Buttons

**Primary Button:**
```css
background: linear-gradient(135deg, #f97316 0%, #fb923c 100%);
color: white;
padding: 15px 40px;
border-radius: 5px;
font-weight: 600;
font-size: 16px;
border: none;
cursor: pointer;
transition: all 0.3s ease;

/* Hover */
transform: translateY(-2px);
box-shadow: 0 5px 15px rgba(249, 115, 22, 0.3);
```

**Secondary Button:**
```css
background: white;
color: #1e3a8a;
padding: 15px 40px;
border-radius: 5px;
font-weight: 600;
font-size: 16px;
border: 2px solid #1e3a8a;
cursor: pointer;
transition: all 0.3s ease;

/* Hover */
background: #1e3a8a;
color: white;
```

**Ghost Button (on dark background):**
```css
background: transparent;
color: white;
padding: 15px 40px;
border-radius: 5px;
font-weight: 600;
font-size: 16px;
border: 2px solid white;
cursor: pointer;
transition: all 0.3s ease;

/* Hover */
background: rgba(255, 255, 255, 0.1);
```

### Cards

**Service Card:**
```css
background: white;
padding: 40px;
border-radius: 10px;
box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
transition: transform 0.3s, box-shadow 0.3s;

/* Hover */
transform: translateY(-5px);
box-shadow: 0 5px 20px rgba(0, 0, 0, 0.1);
```

**Info Card:**
```css
background: #f8fafc;
padding: 30px;
border-radius: 10px;
border-left: 4px solid #f97316;
```

### Forms

**Input Fields:**
```css
width: 100%;
padding: 12px 15px;
border: 2px solid #e2e8f0;
border-radius: 5px;
font-size: 16px;
transition: border-color 0.3s;

/* Focus */
border-color: #3b82f6;
outline: none;
```

**Textarea:**
```css
width: 100%;
padding: 12px 15px;
border: 2px solid #e2e8f0;
border-radius: 5px;
font-size: 16px;
min-height: 120px;
resize: vertical;
```

**Select Dropdown:**
```css
width: 100%;
padding: 12px 15px;
border: 2px solid #e2e8f0;
border-radius: 5px;
font-size: 16px;
background: white;
cursor: pointer;
```

### Navigation

**Top Bar:**
```css
background: #1e3a8a;
color: white;
padding: 10px 0;
font-size: 14px;
```

**Main Navigation:**
```css
background: white;
box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
position: sticky;
top: 0;
z-index: 1000;
```

**Nav Link:**
```css
color: #333;
text-decoration: none;
font-weight: 500;
padding: 10px;
transition: color 0.3s;

/* Hover/Active */
color: #f97316;
```

---

## 🌓 GRADIENTS

### Brand Gradients
```css
/* Primary Gradient (Blue) */
background: linear-gradient(135deg, #1e3a8a 0%, #3b82f6 100%);

/* Accent Gradient (Orange) */
background: linear-gradient(135deg, #f97316 0%, #fb923c 100%);

/* Success Gradient (Green) */
background: linear-gradient(135deg, #10b981 0%, #34d399 100%);
```

---

## 🎯 ICONS & IMAGERY

### Icon System
- **Style:** Outlined or filled (consistent throughout)
- **Size:** 24px default, 32px for larger elements, 48px for features
- **Color:** Match section color scheme
- **Source:** Font Awesome, Lucide Icons, or similar

### Image Guidelines
- **Aspect Ratios:** 16:9 for hero images, 1:1 for team photos, 4:3 for featured images
- **Quality:** High resolution (min 1920px wide for hero)
- **Format:** WebP with JPG fallback, PNG for logos
- **Optimization:** Compress images, lazy load

### Logo Usage
- **Full Color:** On white or light backgrounds
- **White:** On dark or image backgrounds
- **Minimum Size:** 150px wide
- **Clear Space:** Equal to height of logo on all sides

---

## 📱 RESPONSIVE BREAKPOINTS

```css
/* Mobile First Approach */

/* Extra Small (Mobile) */
@media (min-width: 0px) { }

/* Small (Large Mobile) */
@media (min-width: 640px) { }

/* Medium (Tablet) */
@media (min-width: 768px) { }

/* Large (Desktop) */
@media (min-width: 1024px) { }

/* Extra Large (Large Desktop) */
@media (min-width: 1280px) { }

/* 2XL (Ultra Wide) */
@media (min-width: 1536px) { }
```

### Layout Adjustments

**Desktop (1024px+):**
- 3-4 column grids
- Full navigation visible
- 80px section padding

**Tablet (768px-1023px):**
- 2-3 column grids
- Compressed navigation
- 60px section padding

**Mobile (0-767px):**
- Single column layouts
- Hamburger menu
- 40px section padding
- Larger touch targets (min 44px)

---

## ✅ ACCESSIBILITY STANDARDS

### Color Contrast
- **Text on white:** Minimum 4.5:1 ratio
- **Large text (18px+):** Minimum 3:1 ratio
- **Interactive elements:** Minimum 4.5:1 ratio

### Focus States
```css
*:focus {
  outline: 2px solid #3b82f6;
  outline-offset: 2px;
}
```

### Alt Text
- All images must have descriptive alt text
- Decorative images: alt=""
- Informative images: Describe content

### Semantic HTML
- Use proper heading hierarchy (H1 → H2 → H3)
- Use `<nav>`, `<main>`, `<footer>`, `<article>`, `<section>`
- Use `<button>` for actions, `<a>` for navigation

---

## 🎬 ANIMATIONS & TRANSITIONS

### Standard Transitions
```css
transition: all 0.3s ease;
```

### Hover Effects

**Lift Effect:**
```css
transform: translateY(-5px);
transition: transform 0.3s;
```

**Shadow Effect:**
```css
box-shadow: 0 5px 20px rgba(0, 0, 0, 0.1);
transition: box-shadow 0.3s;
```

**Color Change:**
```css
color: #f97316;
transition: color 0.3s;
```

### Loading States
- Use subtle fade-in for content
- Skeleton screens for slow-loading content
- Progress indicators for forms

---

## 📋 DESIGN CHECKLIST

### Before Development
- [ ] All mockups approved
- [ ] Content written and approved
- [ ] Images prepared (optimized)
- [ ] Logo files ready (SVG, PNG)
- [ ] Partner logos collected
- [ ] Brand colors finalized
- [ ] Font selections confirmed

### During Development
- [ ] Follow spacing system
- [ ] Use correct color codes
- [ ] Maintain consistent typography
- [ ] Implement hover states
- [ ] Add focus states
- [ ] Test on mobile devices
- [ ] Check color contrast
- [ ] Validate HTML
- [ ] Optimize images

### Before Launch
- [ ] Cross-browser testing
- [ ] Mobile responsiveness
- [ ] Accessibility audit
- [ ] Performance testing
- [ ] Form functionality
- [ ] Link testing
- [ ] SEO optimization
- [ ] Analytics setup

---

## 🎨 EXAMPLE COMPONENT CODE

### Hero Section
```html
<section class="hero">
  <h1>Your Heading Here</h1>
  <p>Your subheading or description</p>
  <div class="hero-buttons">
    <a href="/contact" class="btn btn-primary">Primary Action</a>
    <a href="/services" class="btn btn-secondary">Secondary Action</a>
  </div>
</section>
```

```css
.hero {
  background: linear-gradient(135deg, #1e3a8a 0%, #3b82f6 100%);
  color: white;
  padding: 100px 20px;
  text-align: center;
}

.hero h1 {
  font-size: 48px;
  margin-bottom: 20px;
}

.hero p {
  font-size: 20px;
  margin-bottom: 30px;
  opacity: 0.9;
}
```

### Service Card
```html
<div class="service-card">
  <div class="service-icon">🎓</div>
  <h3>IT Education</h3>
  <p>World-class training programs and international certifications</p>
  <a href="/services/education" class="service-link">Learn More →</a>
</div>
```

```css
.service-card {
  background: white;
  padding: 40px;
  border-radius: 10px;
  text-align: center;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
  transition: transform 0.3s, box-shadow 0.3s;
}

.service-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 5px 20px rgba(0, 0, 0, 0.1);
}
```

---

## 🔗 QUICK REFERENCE

### Most Used Colors
```
Blue: #1e3a8a
Orange: #f97316
Green: #10b981
Gray: #64748b
White: #ffffff
```

### Most Used Spacing
```
Section Padding: 80px (desktop), 40px (mobile)
Card Padding: 40px
Button Padding: 15px 40px
Grid Gap: 30px
```

### Most Used Font Sizes
```
Hero: 48px
Heading: 36px
Subheading: 24px
Body: 16px
Small: 14px
```

---

**This style guide ensures:**
✅ Visual consistency across all pages  
✅ Faster development time  
✅ Better user experience  
✅ Professional appearance  
✅ Brand coherence  

**Questions? Contact:** design@tripleaconsulting.com.ng