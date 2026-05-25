# Farzam.nl Premium Motion Guide

## Purpose

This document defines the motion and interaction direction for Farzam.nl.

The motion system should make the website feel premium, calm, intelligent, and precise.

Motion should support clarity, not decoration.

The website should feel like:

Apple + McKinsey + Premium SaaS + Strategic Growth Platform

It should not feel like:
- A flashy agency website
- A gaming interface
- A noisy AI startup page
- A template full of random animations
- A website where motion distracts from the message

---

## Core Motion Principle

Motion must be:

- Calm
- Subtle
- Intentional
- Lightweight
- Fast but not aggressive
- Premium
- Clear
- Mobile-friendly

Every animation should answer one question:

Does this make the experience clearer, smoother, or more premium?

If not, remove it.

---

## Motion Hierarchy

Use motion in this order of importance:

1. Page load reveal
2. Section reveal
3. Button hover
4. Card hover
5. Hamburger menu open / close
6. Form step transitions
7. Dashboard card transitions
8. Blog / course card interactions

Avoid using motion just to create excitement.

Farzam.nl should feel confident, not loud.

---

## Recommended Motion Types

### 1. Soft Fade Reveal

Use for:
- Hero text
- Section headings
- Important content blocks
- CTA groups

Behavior:
- Opacity from 0 to 1
- Move slightly upward
- Duration between 600ms and 800ms
- Smooth easing

---

### 2. Gentle Slide Up

Use for:
- Cards
- Module blocks
- Blog cards
- Course cards
- Process steps

Behavior:
- Start 16px to 24px lower
- Move into position
- Avoid large movement

---

### 3. Subtle Hover Lift

Use for:
- Cards
- Buttons
- Resource blocks
- Course cards
- Blog cards

Behavior:
- Move upward by 2px to 4px
- Add slightly stronger shadow
- No scaling above 1.01

---

### 4. Smooth Menu Overlay

Use for:
- Hamburger menu
- Full-screen navigation
- Side menu panel

Behavior:
- Fade overlay in
- Menu links reveal with slight delay
- Close smoothly
- No bounce effect

---

### 5. Form Step Transition

Use for:
- Growth Diagnosis form
- Multi-step contact form
- Newsletter preferences

Behavior:
- Fade between steps
- Small horizontal or vertical movement
- Keep form interaction calm

---

## JavaScript Base Motion Script

Use this as the base script for reveal animations.

```javascript
document.addEventListener("DOMContentLoaded", function () {
  const revealElements = document.querySelectorAll(".fgs-reveal");

  if (!revealElements.length) return;

  const observerOptions = {
    root: null,
    threshold: 0.12,
    rootMargin: "0px 0px -60px 0px"
  };

  const revealObserver = new IntersectionObserver(function (entries, observer) {
    entries.forEach(function (entry) {
      if (entry.isIntersecting) {
        entry.target.classList.add("is-visible");
        observer.unobserve(entry.target);
      }
    });
  }, observerOptions);

  revealElements.forEach(function (element) {
    revealObserver.observe(element);
  });
});
```

---

## Reveal CSS

Use with the JavaScript above.

```css
.fgs-reveal {
  opacity: 0;
  transform: translateY(18px);
  transition:
    opacity 700ms ease,
    transform 700ms ease;
  will-change: opacity, transform;
}

.fgs-reveal.is-visible {
  opacity: 1;
  transform: translateY(0);
}
```

---

## Staggered Reveal

Use staggered reveal for card grids.

Example:
- Module cards
- Blog cards
- Course cards
- Process steps

```css
.fgs-stagger > * {
  opacity: 0;
  transform: translateY(18px);
  transition:
    opacity 700ms ease,
    transform 700ms ease;
}

.fgs-stagger.is-visible > * {
  opacity: 1;
  transform: translateY(0);
}

.fgs-stagger.is-visible > *:nth-child(1) {
  transition-delay: 80ms;
}

.fgs-stagger.is-visible > *:nth-child(2) {
  transition-delay: 140ms;
}

.fgs-stagger.is-visible > *:nth-child(3) {
  transition-delay: 200ms;
}

.fgs-stagger.is-visible > *:nth-child(4) {
  transition-delay: 260ms;
}

.fgs-stagger.is-visible > *:nth-child(5) {
  transition-delay: 320ms;
}

.fgs-stagger.is-visible > *:nth-child(6) {
  transition-delay: 380ms;
}
```

JavaScript support:

```javascript
document.addEventListener("DOMContentLoaded", function () {
  const staggerGroups = document.querySelectorAll(".fgs-stagger");

  if (!staggerGroups.length) return;

  const observerOptions = {
    root: null,
    threshold: 0.12,
    rootMargin: "0px 0px -60px 0px"
  };

  const staggerObserver = new IntersectionObserver(function (entries, observer) {
    entries.forEach(function (entry) {
      if (entry.isIntersecting) {
        entry.target.classList.add("is-visible");
        observer.unobserve(entry.target);
      }
    });
  }, observerOptions);

  staggerGroups.forEach(function (group) {
    staggerObserver.observe(group);
  });
});
```

---

## Button Hover Motion

Buttons should feel premium and precise.

```css
.fgs-btn-primary,
.fgs-btn-secondary {
  transition:
    transform 220ms ease,
    box-shadow 220ms ease,
    background-color 220ms ease,
    border-color 220ms ease,
    color 220ms ease;
}

.fgs-btn-primary:hover,
.fgs-btn-secondary:hover {
  transform: translateY(-1px);
}

.fgs-btn-primary:active,
.fgs-btn-secondary:active {
  transform: translateY(0);
}
```

Avoid:
- Big scaling
- Glow effects
- Neon effects
- Bouncy motion

---

## Card Hover Motion

Cards should feel interactive but not playful.

```css
.fgs-card,
.fgs-blog-card,
.fgs-course-card {
  transition:
    transform 240ms ease,
    box-shadow 240ms ease,
    border-color 240ms ease;
}

.fgs-card:hover,
.fgs-blog-card:hover,
.fgs-course-card:hover {
  transform: translateY(-3px);
  box-shadow: var(--fgs-shadow-soft);
  border-color: var(--fgs-border-strong);
}
```

Avoid:
- Rotation
- 3D flip cards
- Excessive scaling
- Strong shadows

---

## Header Scroll Motion

The header can become slightly more defined after scrolling.

```javascript
document.addEventListener("DOMContentLoaded", function () {
  const header = document.querySelector(".fgs-header");

  if (!header) return;

  function updateHeaderState() {
    if (window.scrollY > 20) {
      header.classList.add("is-scrolled");
    } else {
      header.classList.remove("is-scrolled");
    }
  }

  updateHeaderState();

  window.addEventListener("scroll", updateHeaderState, {
    passive: true
  });
});
```

CSS:

```css
.fgs-header {
  transition:
    background-color 240ms ease,
    box-shadow 240ms ease,
    border-color 240ms ease;
}

.fgs-header.is-scrolled {
  background: rgba(255, 255, 255, 0.94);
  box-shadow: 0 10px 30px rgba(15, 23, 42, 0.05);
  border-bottom-color: rgba(203, 213, 225, 0.9);
}
```

---

## Hamburger Menu Motion

Use a full-screen or large overlay menu.

### HTML Structure Example

```html
<button class="fgs-menu-toggle" aria-label="Open menu">
  Menu
</button>

<div class="fgs-menu-overlay" aria-hidden="true">
  <div class="fgs-menu-panel">
    <button class="fgs-menu-close" aria-label="Close menu">
      Close
    </button>

    <p class="fgs-menu-line">
      Build a Growth System, not just more marketing.
    </p>

    <nav class="fgs-menu-nav">
      <a class="fgs-menu-link" href="/">Home</a>
      <a class="fgs-menu-link" href="/growth-systems">Growth Systems</a>
      <a class="fgs-menu-link" href="/modules">Modules</a>
      <a class="fgs-menu-link" href="/work">Work</a>
      <a class="fgs-menu-link" href="/blog">Blog</a>
      <a class="fgs-menu-link" href="/courses">Courses</a>
      <a class="fgs-menu-link" href="/studio">Studio</a>
      <a class="fgs-menu-link" href="/about">About</a>
      <a class="fgs-menu-link" href="/contact">Contact</a>
    </nav>
  </div>
</div>
```

### JavaScript

```javascript
document.addEventListener("DOMContentLoaded", function () {
  const menuToggle = document.querySelector(".fgs-menu-toggle");
  const menuClose = document.querySelector(".fgs-menu-close");
  const menuOverlay = document.querySelector(".fgs-menu-overlay");
  const menuLinks = document.querySelectorAll(".fgs-menu-link");

  if (!menuToggle || !menuOverlay) return;

  function openMenu() {
    menuOverlay.classList.add("is-open");
    menuOverlay.setAttribute("aria-hidden", "false");
    document.body.classList.add("fgs-menu-is-open");
  }

  function closeMenu() {
    menuOverlay.classList.remove("is-open");
    menuOverlay.setAttribute("aria-hidden", "true");
    document.body.classList.remove("fgs-menu-is-open");
  }

  menuToggle.addEventListener("click", openMenu);

  if (menuClose) {
    menuClose.addEventListener("click", closeMenu);
  }

  menuLinks.forEach(function (link) {
    link.addEventListener("click", closeMenu);
  });

  document.addEventListener("keydown", function (event) {
    if (event.key === "Escape") {
      closeMenu();
    }
  });
});
```

### CSS

```css
body.fgs-menu-is-open {
  overflow: hidden;
}

.fgs-menu-overlay {
  position: fixed;
  inset: 0;
  z-index: 1000;
  background: rgba(255, 255, 255, 0.96);
  backdrop-filter: blur(24px);
  opacity: 0;
  pointer-events: none;
  transition: opacity 260ms ease;
}

.fgs-menu-overlay.is-open {
  opacity: 1;
  pointer-events: auto;
}

.fgs-menu-panel {
  width: min(100% - 32px, 920px);
  margin-inline: auto;
  padding-block: clamp(72px, 10vw, 140px);
}

.fgs-menu-line {
  color: var(--fgs-text-secondary);
  font-size: clamp(1rem, 1.4vw, 1.25rem);
  margin-bottom: 32px;
}

.fgs-menu-link {
  display: block;
  color: var(--fgs-navy-900);
  font-size: clamp(2rem, 5vw, 5rem);
  line-height: 1.05;
  letter-spacing: -0.05em;
  text-decoration: none;
  padding-block: 10px;
  border-bottom: 1px solid var(--fgs-border);
  opacity: 0;
  transform: translateY(14px);
  transition:
    opacity 360ms ease,
    transform 360ms ease,
    color 200ms ease;
}

.fgs-menu-overlay.is-open .fgs-menu-link {
  opacity: 1;
  transform: translateY(0);
}

.fgs-menu-overlay.is-open .fgs-menu-link:nth-child(1) {
  transition-delay: 80ms;
}

.fgs-menu-overlay.is-open .fgs-menu-link:nth-child(2) {
  transition-delay: 120ms;
}

.fgs-menu-overlay.is-open .fgs-menu-link:nth-child(3) {
  transition-delay: 160ms;
}

.fgs-menu-overlay.is-open .fgs-menu-link:nth-child(4) {
  transition-delay: 200ms;
}

.fgs-menu-overlay.is-open .fgs-menu-link:nth-child(5) {
  transition-delay: 240ms;
}

.fgs-menu-overlay.is-open .fgs-menu-link:nth-child(6) {
  transition-delay: 280ms;
}

.fgs-menu-overlay.is-open .fgs-menu-link:nth-child(7) {
  transition-delay: 320ms;
}

.fgs-menu-overlay.is-open .fgs-menu-link:nth-child(8) {
  transition-delay: 360ms;
}

.fgs-menu-overlay.is-open .fgs-menu-link:nth-child(9) {
  transition-delay: 400ms;
}

.fgs-menu-link:hover {
  color: var(--fgs-blue-600);
}
```

---

## Form Step Motion

Use this for multi-step Growth Diagnosis forms.

```css
.fgs-form-step {
  opacity: 0;
  transform: translateY(12px);
  pointer-events: none;
  transition:
    opacity 280ms ease,
    transform 280ms ease;
  display: none;
}

.fgs-form-step.is-active {
  display: block;
  opacity: 1;
  transform: translateY(0);
  pointer-events: auto;
}
```

Example JavaScript:

```javascript
document.addEventListener("DOMContentLoaded", function () {
  const forms = document.querySelectorAll(".fgs-multistep-form");

  forms.forEach(function (form) {
    const steps = form.querySelectorAll(".fgs-form-step");
    const nextButtons = form.querySelectorAll("[data-next-step]");
    const prevButtons = form.querySelectorAll("[data-prev-step]");

    let currentStep = 0;

    function showStep(index) {
      steps.forEach(function (step, stepIndex) {
        step.classList.toggle("is-active", stepIndex === index);
      });
    }

    nextButtons.forEach(function (button) {
      button.addEventListener("click", function () {
        if (currentStep < steps.length - 1) {
          currentStep += 1;
          showStep(currentStep);
        }
      });
    });

    prevButtons.forEach(function (button) {
      button.addEventListener("click", function () {
        if (currentStep > 0) {
          currentStep -= 1;
          showStep(currentStep);
        }
      });
    });

    showStep(currentStep);
  });
});
```

---

## Dashboard Motion

Dashboard motion should be extremely subtle.

Use for:
- Dashboard cards
- Course cards
- Saved resources
- Diagnosis status card

```css
.fgs-dashboard-card {
  transition:
    transform 220ms ease,
    box-shadow 220ms ease,
    border-color 220ms ease;
}

.fgs-dashboard-card:hover {
  transform: translateY(-2px);
  box-shadow: var(--fgs-shadow-card);
  border-color: var(--fgs-border-strong);
}
```

---

## Page Transition Direction

Do not use heavy page transitions in the MVP.

Recommended:
- Keep normal page loading
- Use section reveal after page load
- Avoid full-page loaders
- Avoid spinning logos
- Avoid artificial waiting screens

If page transitions are added later, they must be:
- Very short
- Clean
- Accessible
- Non-blocking

---

## Motion Accessibility

Always respect reduced motion preferences.

```css
@media (prefers-reduced-motion: reduce) {
  *,
  *::before,
  *::after {
    animation-duration: 0.001ms !important;
    animation-iteration-count: 1 !important;
    scroll-behavior: auto !important;
    transition-duration: 0.001ms !important;
  }

  .fgs-reveal,
  .fgs-stagger > *,
  .fgs-menu-link {
    opacity: 1 !important;
    transform: none !important;
  }
}
```

---

## Elementor Implementation Notes

In Elementor:

Use classes:
- `fgs-reveal` for individual reveal elements
- `fgs-stagger` for card grids
- `fgs-card` for standard cards
- `fgs-btn-primary` for main CTA buttons
- `fgs-btn-secondary` for secondary buttons
- `fgs-header` for global header
- `fgs-menu-overlay` for menu overlay
- `fgs-dashboard-card` for dashboard cards

Where to add JavaScript:
- Elementor Custom Code
- Theme custom JS area
- Code Snippets plugin
- Child theme if needed later

Where to add CSS:
- Elementor Site Settings Custom CSS
- Elementor Custom CSS
- Theme customizer
- Child theme stylesheet if needed later

---

## Motion by Page

### Home

Use:
- Hero reveal
- Section reveal
- Module card stagger
- CTA hover

Avoid:
- Too many animations above the fold

---

### Growth Systems

Use:
- Framework diagram reveal
- Process step stagger
- Calm transitions

Avoid:
- Overcomplicated system animation

---

### Modules

Use:
- Card hover
- Staggered module reveal

Avoid:
- Card flipping or 3D effects

---

### Work

Use:
- Case study card reveal
- Proof point reveal

Avoid:
- Portfolio-style flashy transitions

---

### Blog

Use:
- Blog card hover
- Category filter soft transition

Avoid:
- Infinite motion effects

---

### Courses

Use:
- Course card reveal
- Webinar block reveal
- Resource hover

Avoid:
- Gamified animations

---

### Studio

Use:
- Philosophy block reveal
- Process reveal
- Capability card hover

Avoid:
- Agency-style flashy animation

---

### About

Use:
- Calm portrait reveal
- Philosophy text reveal
- Proof point reveal

Avoid:
- Overanimated biography timeline

---

### Contact

Use:
- Form step transition
- CTA card hover
- Booking section reveal

Avoid:
- Distracting animation around forms

---

### Dashboard

Use:
- Very subtle dashboard card hover
- Calm tab transitions

Avoid:
- Gamification, badges, noisy progress animation

---

## Motion Do Not Use List

Do not use:

- Neon glow effects
- Fast spinning icons
- Bouncy animation
- Heavy parallax
- 3D card flips
- Aggressive scroll hijacking
- Auto-moving carousels
- Flashy AI particles
- Unnecessary loading screens
- Animation that delays the user

---

## Final Motion Rule

Motion on Farzam.nl should feel like a confident consultant entering a room.

Calm. Precise. Clear. Premium.

Nothing should shout.

Everything should support trust.
