# Elementor Implementation Guide

## Purpose

This document explains how to implement Farzam.nl inside WordPress and Elementor Pro based on the existing project documentation.

The website should be built as a premium Growth System platform, not as a generic personal portfolio or marketing agency website.

The goal is to translate all page blueprints, components, design direction, SEO architecture, and automation logic into a clean Elementor implementation.

---

## Core Positioning Reminder

Farzam.nl must position Farzam as:

- Growth Strategist
- Growth System Designer
- Business-Oriented Thinker

The website must not position him as:

- Traditional marketer
- Freelance marketer
- Social media manager
- AI tool operator
- Generic agency owner

Core message:

Build a Growth System, not just more marketing.

---

## Website Stack

Recommended stack:

- WordPress
- Elementor Pro
- Yoast SEO
- WooCommerce if needed later
- Membership plugin for account system
- LMS plugin for courses later
- n8n for automation workflows

Possible account / membership plugins:

- Ultimate Member
- ProfilePress
- Paid Memberships Pro

Possible LMS plugins:

- Tutor LMS
- LearnDash
- LifterLMS

Possible booking tools:

- Calendly
- FluentBooking
- Amelia

---

## Required Main Pages

Create these WordPress pages:

1. Home
   - URL: `/`

2. Growth Systems
   - URL: `/growth-systems`

3. Modules
   - URL: `/modules`

4. Work
   - URL: `/work`

5. Blog
   - URL: `/blog`

6. Courses
   - URL: `/courses`

7. Studio
   - URL: `/studio`

8. About
   - URL: `/about`

9. Contact
   - URL: `/contact`

10. Dashboard
   - URL: `/dashboard`

11. Register
   - URL: `/register`

12. Sign In
   - URL: `/login`

---

## Blueprint Reference Files

Use these files as the content and layout source:

- `elementor/page-blueprints/HOME.md`
- `elementor/page-blueprints/GROWTH_SYSTEMS.md`
- `elementor/page-blueprints/MODULES.md`
- `elementor/page-blueprints/WORK.md`
- `elementor/page-blueprints/BLOG.md`
- `elementor/page-blueprints/COURSES.md`
- `elementor/page-blueprints/STUDIO.md`
- `elementor/page-blueprints/ABOUT.md`
- `elementor/page-blueprints/CONTACT.md`
- `elementor/page-blueprints/DASHBOARD.md`

Use these files as global component references:

- `elementor/components/HEADER_NAVIGATION.md`
- `elementor/components/FOOTER.md`

Use these files for styling and motion:

- `elementor/custom-css/FARZAM_GLOBAL_STYLE.md`
- `elementor/custom-js/FARZAM_PREMIUM_MOTION.md`

---

## Elementor Global Setup

Before designing pages, configure Elementor Site Settings.

### Global Colors

Use the color system from:

`elementor/custom-css/FARZAM_GLOBAL_STYLE.md`

Core colors:

- Navy
- Deep blue
- White
- Soft light background
- Warm neutral
- Muted gray text
- Subtle gold accent

### Global Typography

Recommended font direction:

- Inter
- Manrope
- Satoshi
- System sans-serif fallback

Typography should feel:

- Premium
- Modern
- Clean
- Executive
- Editorial
- Easy to read

### Global Layout

Recommended max widths:

- Standard container: 1180px
- Wide container: 1320px

Use spacious sections and strong white space.

Avoid cramped layouts.

---

## Global Header Implementation

Use Elementor Pro Theme Builder.

Create:

`Global Header`

Use reference:

`elementor/components/HEADER_NAVIGATION.md`

Visible header structure:

- Logo
- Hamburger Menu
- Register / Sign In
- Book a Strategy Call

Header behavior:

- Sticky
- Minimal
- Light background
- Slight blur or solid white on scroll
- Premium spacing
- Mobile optimized

The hamburger menu should include all main site pages.

---

## Global Footer Implementation

Use Elementor Pro Theme Builder.

Create:

`Global Footer`

Use reference:

`elementor/components/FOOTER.md`

Footer should include:

- Brand block
- Main navigation
- Growth topics
- Courses and resources
- Newsletter signup
- Contact CTA
- Social links
- Legal links

Footer should support:

- SEO internal linking
- Newsletter growth
- Conversion
- Trust

---

## Page Building Order

Build pages in this order:

1. Header
2. Footer
3. Home
4. Growth Systems
5. Modules
6. Work
7. Blog
8. Courses
9. Studio
10. About
11. Contact
12. Dashboard
13. Register
14. Login

Reason:

The header and footer define the global structure first.  
The Home page then introduces the full system.  
The other pages expand the platform step by step.

---

## Home Page Implementation

Use:

`elementor/page-blueprints/HOME.md`

The Home page should explain:

- Who Farzam helps
- What Growth Systems are
- Why scattered marketing is not enough
- How Farzam’s approach works
- What the visitor should do next

Hero should include:

- Strong positioning
- Clear CTA
- Premium visual system
- No generic marketing language

Primary CTA:

Book a Strategy Call

Secondary CTA:

Explore Growth Systems

---

## Growth Systems Page Implementation

Use:

`elementor/page-blueprints/GROWTH_SYSTEMS.md`

This is one of the most important pages.

It must explain the methodology behind the brand.

The page should clarify:

- What a Growth System is
- Why businesses need one
- How the system works
- Why marketing and AI are only parts of the system

Use diagrams, process blocks, and clean explanatory sections.

---

## Modules Page Implementation

Use:

`elementor/page-blueprints/MODULES.md`

This page should show Farzam’s strategic capability areas.

Each module should feel like part of a larger system, not an isolated service.

Avoid service-page clutter.

Use clean module cards.

---

## Work Page Implementation

Use:

`elementor/page-blueprints/WORK.md`

This page should build credibility.

It should not feel like a generic portfolio gallery.

Each work item should show:

- Context
- Problem
- Strategic role
- System contribution
- Outcome or strategic value

---

## Blog Page Implementation

Use:

`elementor/page-blueprints/BLOG.md`

The blog should support thought leadership and SEO.

Important:

SEO is not the topic of the blog.  
SEO is the structure behind the blog.

Blog categories should include:

- Growth Systems
- Brand Positioning
- AI Leverage
- Customer Journey
- Content Systems
- Business Clarity
- Personal Brand

---

## Courses Page Implementation

Use:

`elementor/page-blueprints/COURSES.md`

The Courses page should support:

- Free courses
- Paid courses
- Webinars
- Workshops
- Lead magnets
- Register / Sign In
- YouTube and Skool audience entry
- Course-to-consulting conversion

Courses should connect education to strategic consulting.

---

## Studio Page Implementation

Use:

`elementor/page-blueprints/STUDIO.md`

This page should explain Farzam Growth Studio as the ecosystem behind the work.

It should not sound like a traditional agency.

Core idea:

System first. Marketing second. AI only when useful.

---

## About Page Implementation

Use:

`elementor/page-blueprints/ABOUT.md`

The About page should build credibility and human trust.

It should not be a traditional CV page.

It should explain:

- Who Farzam is
- How he thinks
- His background
- Why he builds Growth Systems
- Why his experience is relevant

---

## Contact Page Implementation

Use:

`elementor/page-blueprints/CONTACT.md`

The Contact page should include:

- Strategy call CTA
- Growth Diagnosis form
- General contact form
- Course / webinar inquiry path
- Collaboration inquiry path

The contact page must feel like the start of a serious strategic conversation.

---

## Dashboard Implementation

Use:

`elementor/page-blueprints/DASHBOARD.md`

The dashboard should support:

- My Courses
- My Webinars
- Saved Resources
- Growth Diagnosis Status
- Newsletter Preferences
- Member-only Strategy Offer
- Account Settings

Dashboard should be noindex.

The dashboard may require a membership plugin and custom templates.

---

## Register and Login Pages

Create simple, premium account pages.

### Register Page

URL:

`/register`

Purpose:

Allow users to create an account for courses, webinars, saved resources, dashboard access, and newsletter preferences.

Include:

- Name
- Email
- Password
- Consent checkbox
- Interest category if possible

After registration:

Redirect to:

`/dashboard`

### Login Page

URL:

`/login`

Purpose:

Allow existing users to access their account.

After login:

Redirect to:

`/dashboard`

---

## Forms

Recommended forms:

1. Growth Diagnosis Form
2. Contact Form
3. Newsletter Signup Form
4. Course Interest Form
5. Webinar Registration Form
6. Strategy Call Request Form

Forms should be:

- Clean
- Premium
- Mobile-friendly
- Not overwhelming
- Connected to n8n later

For long forms, use multi-step layout.

---

## n8n Integration Direction

All important user actions should eventually connect to n8n.

Important triggers:

- Newsletter subscription
- Growth Diagnosis submission
- Contact form submission
- Course registration
- Webinar registration
- Strategy call booking
- Dashboard activity
- Resource download
- Member offer click

n8n should support:

- Email confirmation
- Lead segmentation
- CRM updates
- Follow-up sequences
- Course-to-consulting conversion
- Newsletter preference management

---

## SEO Implementation

Use:

`seo/SEO_ARCHITECTURE.md`

For each page:

- One clear H1
- Clean URL slug
- SEO title
- Meta description
- Internal links
- Structured headings
- Topic consistency
- No keyword stuffing

Important:

Dashboard, login, register, and account pages should usually be noindex.

Blog posts should be SEO structured.

---

## Design System Implementation

Use:

`design-system/DESIGN_SYSTEM.md`

Visual style should be:

- Premium
- Minimal
- Executive
- Spacious
- White / light
- Strategic
- Calm
- Trustworthy

Avoid:

- Noisy gradients
- Generic stock images
- Heavy AI visuals
- Loud agency graphics
- Dark tech cliché design

---

## Motion Implementation

Use:

`elementor/custom-js/FARZAM_PREMIUM_MOTION.md`

Apply motion carefully.

Recommended classes:

- `fgs-reveal`
- `fgs-stagger`
- `fgs-card`
- `fgs-btn-primary`
- `fgs-btn-secondary`

Motion must be:

- Calm
- Subtle
- Lightweight
- Accessible
- Non-distracting

---

## Mobile Implementation

Every page must be mobile optimized.

Mobile priorities:

- Clear hero
- Readable typography
- Large tap targets
- Simple navigation
- Clean forms
- No overcrowded sections
- Fast loading
- Dashboard usability

---

## Performance Requirements

Keep the website fast.

Avoid:

- Heavy animation libraries
- Too many plugins
- Large uncompressed images
- Unnecessary sliders
- Auto-playing videos
- Excessive custom code

Use:

- Optimized images
- Lightweight CSS
- Minimal JavaScript
- Lazy loading
- Clean Elementor structure

---

## Accessibility Requirements

Website should include:

- Good color contrast
- Keyboard accessible navigation
- Clear focus states
- Form labels
- Accessible buttons
- Proper heading hierarchy
- Reduced motion support

---

## Final Implementation Rule

Every page should answer three questions clearly:

1. What is this page for?
2. What does the visitor learn here?
3. What should the visitor do next?

The website should feel like a structured Growth System.

Not a portfolio.

Not an agency site.

Not an AI tool website.

A premium strategic platform built around Farzam’s thinking, methodology, education, and consulting path.
