# Fluventa Technologies - Website Specification

## 1. Project Overview

**Project Name:** Fluventa Technologies Website  
**Project Type:** Single-page digital agency website  
**Core Functionality:** A premium, award-winning level website showcasing Fluventa Technologies' digital services with immersive UI, smooth animations, and conversion-optimized structure.  
**Target Users:** Potential clients in Kenya and globally seeking web development, UI/UX design, SEO, automation, and branding services.

---

## 2. UI/UX Specification

### Layout Structure

**Page Sections (in order):**
1. Navigation (sticky)
2. Hero Section
3. About Section
4. Services Section
5. Process Section
6. Portfolio Section
7. Testimonials Section
8. Pricing Section
9. Contact Section
10. Footer

**Responsive Breakpoints:**
- Mobile: 320px - 767px
- Tablet: 768px - 1023px
- Desktop: 1024px+

### Visual Design

**Color Palette:**
- Primary: #0066ff (Electric Blue)
- Secondary: #00c6ff (Cyan)
- Accent: #7f5af0 (Purple)
- Background Primary: #0f172a (Dark Navy)
- Background Secondary: #1e293b (Slate)
- Text Primary: #f8fafc (Off-white)
- Text Secondary: #94a3b8 (Muted gray)
- Success: #10b981 (Emerald)
- Error: #ef4444 (Red)

**Typography:**
- Headings: "Outfit" (Google Fonts) - weights 600, 700, 800
- Body: "Plus Jakarta Sans" (Google Fonts) - weights 400, 500, 600
- Hero Headline: 4rem (desktop), 2.5rem (mobile)
- Section Titles: 3rem (desktop), 2rem (mobile)
- Body Text: 1rem
- Small Text: 0.875rem

**Spacing System:**
- Section Padding: 100px vertical (desktop), 60px (mobile)
- Container Max Width: 1200px
- Grid Gap: 30px
- Card Padding: 40px

**Visual Effects:**
- Glassmorphism: backdrop-filter: blur(20px); background: rgba(30, 41, 59, 0.7)
- Glow Effects: box-shadow: 0 0 40px rgba(0, 102, 255, 0.3)
- Gradient Overlays: linear-gradient(135deg, #0066ff 0%, #7f5af0 100%)
- Border Radius: 16px (cards), 8px (buttons), 50% (avatars)

### Components

**Navigation:**
- Logo (left)
- Menu links (center): Home, About, Services, Portfolio, Pricing, Contact
- CTA Button (right): "Get Started"
- Mobile: Hamburger menu with slide-in drawer
- Active state: Glowing underline effect

**Hero Section:**
- Animated gradient background with floating orbs
- Headline with typing or fade-in animation
- Subtext with staggered reveal
- Two CTA buttons with hover glow
- Scroll indicator at bottom

**Service Cards:**
- Glassmorphic background
- Icon (SVG with glow)
- Title and description
- Hover: Scale up, border glow, icon animation

**Portfolio Items:**
- Image with overlay on hover
- Project title and tech stack
- Modal popup for details

**Testimonial Carousel:**
- Auto-sliding (5s interval)
- Navigation dots
- Client photo, name, role, quote

**Pricing Cards:**
- Three tiers: Starter, Professional, Enterprise
- Featured card (Professional) with highlight
- Feature list with checkmarks
- CTA button

**Contact Form:**
- Floating labels
- Validation states
- Submit button with loading state
- Success/error messages

**Floating Chatbot:**
- Fixed position bottom-right
- Pulsing animation
- Opens chat modal on click

---

## 3. Functionality Specification

### Core Features

1. **Smooth Scrolling Navigation**
   - Click nav links to smooth scroll to sections
   - Active section highlighting in nav

2. **Scroll-Triggered Animations**
   - Elements fade/slide in when entering viewport
   - Staggered animations for lists and grids
   - Uses Intersection Observer API

3. **Animated Counters**
   - Numbers count up when in viewport
   - Duration: 2 seconds
   - Easing: ease-out

4. **Testimonial Carousel**
   - Auto-advance every 5 seconds
   - Manual navigation with dots
   - Pause on hover

5. **Portfolio Modal**
   - Click project to open modal
   - Image, description, technologies
   - Close on overlay click or X button

6. **Contact Form Validation**
   - Name: Required, min 2 characters
   - Email: Required, valid format
   - Service: Required selection
   - Message: Required, min 10 characters

7. **WhatsApp Integration**
   - Click to open wa.me link
   - Pre-filled message template
   - Format: +254712345678

8. **Dark Mode Toggle**
   - Switch between dark/light themes
   - Persist preference in localStorage
   - Smooth transition

9. **Mobile Menu**
   - Hamburger icon toggle
   - Slide-in from right
   - Close on link click

### User Interactions

- **Hover States:** All interactive elements have clear hover feedback
- **Focus States:** Keyboard navigation support with visible focus rings
- **Loading States:** Buttons show spinner during form submission
- **Scroll Behavior:** Smooth scroll with optional parallax effects

### Edge Cases

- Handle missing images with placeholder
- Form submission shows success message (no backend)
- Carousel handles single testimonial
- Mobile menu closes on resize to desktop

---

## 4. Acceptance Criteria

### Visual Checkpoints
- [ ] Dark theme with blue/purple accents visible
- [ ] Glassmorphic cards render correctly
- [ ] All fonts load properly
- [ ] Animations are smooth (60fps)
- [ ] Mobile layout is fully responsive
- [ ] All sections visible and properly spaced

### Functional Checkpoints
- [ ] Navigation smooth scrolls to sections
- [ ] Active nav item highlights on scroll
- [ ] Service cards animate on hover
- [ ] Portfolio modal opens/closes correctly
- [ ] Testimonial carousel auto-advances
- [ ] Form validates all fields
- [ ] WhatsApp link opens correctly
- [ ] Mobile menu works
- [ ] Scroll animations trigger properly
- [ ] Animated counters work

### Performance Checkpoints
- [ ] Page loads without errors
- [ ] No console errors
- [ ] Images lazy load
- [ ] Smooth scrolling performance

---

## 5. Technical Implementation

**Tech Stack:**
- HTML5 (semantic, accessible)
- CSS3 (custom properties, grid, flexbox, animations)
- JavaScript (ES6+, Intersection Observer, localStorage)
- No external frameworks (vanilla implementation)

**External Resources:**
- Google Fonts: Outfit, Plus Jakarta Sans
- Lucide Icons (CDN)
- Placeholder images from picsum.photos

**Browser Support:**
- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
