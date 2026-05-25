# Farzam.nl Global Style Guide

## Purpose

This document defines the global CSS and styling direction for Farzam.nl.

The goal is to keep the website premium, minimal, executive, calm, and system-oriented.

The style should support:
- WordPress
- Elementor Pro
- Responsive layouts
- Global colors
- Global typography
- Premium motion
- Reusable components
- SEO-friendly structure
- Conversion-focused CTAs

---

## Core Visual Principle

Farzam.nl should feel like:

Apple + McKinsey + Premium SaaS + Independent Growth Strategy Consultant

It should not feel like:
- A generic marketing agency
- A freelancer portfolio
- A social media manager website
- An AI tool website
- A noisy startup template

---

## Global Color Tokens

Use the logo direction as the visual anchor.

```css
:root {
  --fgs-navy-900: #0B1F3A;
  --fgs-navy-800: #102A46;
  --fgs-blue-700: #163B5C;
  --fgs-blue-600: #245C8F;
  --fgs-blue-500: #2F6FA8;

  --fgs-white: #FFFFFF;
  --fgs-bg-light: #F7F9FC;
  --fgs-bg-soft: #F3F6FA;
  --fgs-warm-neutral: #F5F1EA;

  --fgs-text-primary: #111827;
  --fgs-text-secondary: #4B5563;
  --fgs-text-muted: #6B7280;

  --fgs-border: #E5E7EB;
  --fgs-border-strong: #CBD5E1;

  --fgs-accent-gold: #B8945E;
  --fgs-accent-sand: #C7A46B;

  --fgs-radius-sm: 10px;
  --fgs-radius-md: 16px;
  --fgs-radius-lg: 24px;
  --fgs-radius-xl: 32px;

  --fgs-shadow-soft: 0 12px 40px rgba(15, 23, 42, 0.06);
  --fgs-shadow-card: 0 8px 28px rgba(15, 23, 42, 0.05);

  --fgs-container: 1180px;
  --fgs-container-wide: 1320px;
}
```

---

## Typography Direction

Use a modern sans-serif font system.

Recommended:
- Inter
- Manrope
- Satoshi
- Helvetica Neue / system sans-serif

Fallback:

```css
body {
  font-family: Inter, Manrope, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
}
```

---

## Global Body Style

```css
body {
  background: var(--fgs-white);
  color: var(--fgs-text-primary);
  font-size: 16px;
  line-height: 1.7;
  letter-spacing: -0.01em;
  -webkit-font-smoothing: antialiased;
  text-rendering: optimizeLegibility;
}
```

---

## Headings

```css
h1,
h2,
h3,
h4,
h5,
h6 {
  color: var(--fgs-navy-900);
  font-weight: 650;
  letter-spacing: -0.04em;
  line-height: 1.08;
  margin: 0 0 0.65em;
}

h1 {
  font-size: clamp(3rem, 7vw, 6.5rem);
  max-width: 980px;
}

h2 {
  font-size: clamp(2.2rem, 4vw, 4.2rem);
  max-width: 860px;
}

h3 {
  font-size: clamp(1.35rem, 2vw, 2rem);
}
```

---

## Paragraphs

```css
p {
  color: var(--fgs-text-secondary);
  font-size: clamp(1rem, 1.1vw, 1.125rem);
  line-height: 1.75;
  margin: 0 0 1.2em;
}

.fgs-lead {
  font-size: clamp(1.15rem, 1.6vw, 1.45rem);
  line-height: 1.65;
  color: var(--fgs-text-secondary);
  max-width: 780px;
}
```

---

## Containers

```css
.fgs-container {
  width: min(100% - 40px, var(--fgs-container));
  margin-inline: auto;
}

.fgs-container-wide {
  width: min(100% - 40px, var(--fgs-container-wide));
  margin-inline: auto;
}
```

---

## Section Spacing

```css
.fgs-section {
  padding-block: clamp(80px, 9vw, 150px);
}

.fgs-section-compact {
  padding-block: clamp(56px, 6vw, 96px);
}

.fgs-section-soft {
  background: var(--fgs-bg-light);
}
```

Mobile rule:
- Reduce spacing, but do not make sections feel cramped.
- Keep strong vertical rhythm.

---

## Header Style

```css
.fgs-header {
  position: sticky;
  top: 0;
  z-index: 999;
  background: rgba(255, 255, 255, 0.88);
  backdrop-filter: blur(18px);
  border-bottom: 1px solid rgba(229, 231, 235, 0.75);
}

.fgs-header-inner {
  width: min(100% - 32px, var(--fgs-container-wide));
  margin-inline: auto;
  height: 76px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.fgs-logo {
  display: flex;
  align-items: center;
  gap: 12px;
}

.fgs-header-actions {
  display: flex;
  align-items: center;
  gap: 14px;
}
```

---

## Buttons

### Primary Button

```css
.fgs-btn-primary {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  min-height: 48px;
  padding: 0 22px;
  border-radius: 999px;
  background: var(--fgs-navy-900);
  color: var(--fgs-white);
  font-weight: 600;
  text-decoration: none;
  border: 1px solid var(--fgs-navy-900);
  transition: transform 220ms ease, box-shadow 220ms ease, background 220ms ease;
}

.fgs-btn-primary:hover {
  transform: translateY(-1px);
  box-shadow: var(--fgs-shadow-card);
  background: var(--fgs-navy-800);
}
```

### Secondary Button

```css
.fgs-btn-secondary {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  min-height: 48px;
  padding: 0 22px;
  border-radius: 999px;
  background: transparent;
  color: var(--fgs-navy-900);
  font-weight: 600;
  text-decoration: none;
  border: 1px solid var(--fgs-border-strong);
  transition: background 220ms ease, border-color 220ms ease, transform 220ms ease;
}

.fgs-btn-secondary:hover {
  background: var(--fgs-bg-light);
  border-color: var(--fgs-navy-900);
  transform: translateY(-1px);
}
```

---

## Cards

```css
.fgs-card {
  background: var(--fgs-white);
  border: 1px solid var(--fgs-border);
  border-radius: var(--fgs-radius-lg);
  padding: clamp(24px, 3vw, 36px);
  box-shadow: var(--fgs-shadow-card);
  transition: transform 240ms ease, box-shadow 240ms ease, border-color 240ms ease;
}

.fgs-card:hover {
  transform: translateY(-3px);
  border-color: var(--fgs-border-strong);
  box-shadow: var(--fgs-shadow-soft);
}
```

---

## Forms

```css
.fgs-form input,
.fgs-form textarea,
.fgs-form select {
  width: 100%;
  border: 1px solid var(--fgs-border);
  border-radius: var(--fgs-radius-md);
  padding: 14px 16px;
  background: var(--fgs-white);
  color: var(--fgs-text-primary);
  font-size: 1rem;
  transition: border-color 200ms ease, box-shadow 200ms ease;
}

.fgs-form input:focus,
.fgs-form textarea:focus,
.fgs-form select:focus {
  outline: none;
  border-color: var(--fgs-blue-600);
  box-shadow: 0 0 0 4px rgba(36, 92, 143, 0.12);
}

.fgs-form label {
  display: block;
  margin-bottom: 8px;
  color: var(--fgs-navy-900);
  font-weight: 600;
}
```

---

## Hamburger Menu

```css
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
  padding-block: clamp(80px, 10vw, 140px);
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
  transition: color 200ms ease, transform 200ms ease;
}

.fgs-menu-link:hover {
  color: var(--fgs-blue-600);
  transform: translateX(6px);
}
```

---

## Dashboard UI

```css
.fgs-dashboard {
  background: var(--fgs-bg-light);
  min-height: 100vh;
  padding-block: clamp(48px, 6vw, 96px);
}

.fgs-dashboard-grid {
  display: grid;
  grid-template-columns: 280px 1fr;
  gap: 32px;
}

.fgs-dashboard-card {
  background: var(--fgs-white);
  border: 1px solid var(--fgs-border);
  border-radius: var(--fgs-radius-lg);
  padding: 28px;
}

@media (max-width: 768px) {
  .fgs-dashboard-grid {
    grid-template-columns: 1fr;
  }
}
```

---

## Footer

```css
.fgs-footer {
  background: var(--fgs-navy-900);
  color: var(--fgs-white);
  padding-block: clamp(72px, 8vw, 120px) 36px;
}

.fgs-footer a {
  color: rgba(255, 255, 255, 0.78);
  text-decoration: none;
}

.fgs-footer a:hover {
  color: var(--fgs-white);
}

.fgs-footer p {
  color: rgba(255, 255, 255, 0.68);
}
```

---

## Motion Classes

```css
.fgs-reveal {
  opacity: 0;
  transform: translateY(18px);
  transition: opacity 700ms ease, transform 700ms ease;
}

.fgs-reveal.is-visible {
  opacity: 1;
  transform: translateY(0);
}
```

Reduced motion:

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
}
```

---

## Responsive Rules

```css
@media (max-width: 1024px) {
  .fgs-section {
    padding-block: 88px;
  }
}

@media (max-width: 768px) {
  .fgs-container,
  .fgs-container-wide {
    width: min(100% - 28px, var(--fgs-container));
  }

  .fgs-header-inner {
    height: 68px;
  }

  .fgs-header-actions {
    gap: 10px;
  }

  .fgs-btn-primary,
  .fgs-btn-secondary {
    min-height: 44px;
    padding: 0 16px;
  }
}
```

---

## Elementor Usage Notes

Use this global style as a reference for:

- Site Settings
- Global Colors
- Global Fonts
- Custom CSS
- Reusable section classes
- Button classes
- Card classes
- Form classes
- Dashboard classes
- Header and footer styling

In Elementor, assign classes like:

- `fgs-section`
- `fgs-container`
- `fgs-card`
- `fgs-btn-primary`
- `fgs-btn-secondary`
- `fgs-reveal`

---

## Final Rule

The styling should make the website feel:

- Strategic
- Calm
- Premium
- Structured
- Human
- Precise
- Trustworthy

The design should never compete with the message. It should make the message clearer.
