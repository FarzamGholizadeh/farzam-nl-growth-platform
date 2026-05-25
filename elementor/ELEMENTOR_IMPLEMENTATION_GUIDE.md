# Elementor Implementation Guide

## Purpose

This document explains how to implement Farzam.nl inside WordPress and Elementor Pro based on the existing project documentation.

The website should be built as a premium Growth System platform, not as a generic personal portfolio, marketing agency website, or AI landing page.

The goal is to translate all page blueprints, components, design direction, SEO architecture, copywriting rules, and automation logic into a clean Elementor implementation.

---

## Core Positioning Reminder

Farzam.nl must position Farzam as:

1. Growth Strategist
2. Growth System Designer
3. Business-Oriented Thinker

The website must not position him as:

1. Traditional marketer
2. Freelance marketer
3. Social media manager
4. AI tool operator
5. Generic agency owner

Core message:

Build a Growth System, not just more marketing.

Marketing, content, AI, automation, and websites are tools inside the Growth System.

They are not the identity of the brand.

---

## Website Stack

Recommended stack:

1. WordPress
2. Elementor Pro
3. Yoast SEO
4. n8n
5. Membership plugin later
6. LMS plugin later
7. Booking tool
8. Newsletter and CRM integration
9. WooCommerce only if needed later

Possible account and membership plugins:

1. Ultimate Member
2. ProfilePress
3. Paid Memberships Pro

Possible LMS plugins:

1. Tutor LMS
2. LearnDash
3. LifterLMS

Possible booking tools:

1. Calendly
2. FluentBooking
3. Amelia

---

## Required Main Pages

Create these WordPress pages:

1. Home
   URL: `/`

2. Growth Systems
   URL: `/growth-systems`

3. Modules
   URL: `/modules`

4. Work
   URL: `/work`

5. Blog
   URL: `/blog`

6. Courses
   URL: `/courses`

7. Studio
   URL: `/studio`

8. About
   URL: `/about`

9. Contact
   URL: `/contact`

10. Dashboard
   URL: `/dashboard`

11. Register
   URL: `/register`

12. Sign In
   URL: `/login`

---

## Blueprint Reference Files

Use these files as the content and layout source:

1. `elementor/page-blueprints/HOME.md`
2. `elementor/page-blueprints/GROWTH_SYSTEMS.md`
3. `elementor/page-blueprints/MODULES.md`
4. `elementor/page-blueprints/WORK.md`
5. `elementor/page-blueprints/BLOG.md`
6. `elementor/page-blueprints/COURSES.md`
7. `elementor/page-blueprints/STUDIO.md`
8. `elementor/page-blueprints/ABOUT.md`
9. `elementor/page-blueprints/CONTACT.md`
10. `elementor/page-blueprints/DASHBOARD.md`

Use these files as global component references:

1. `elementor/components/HEADER_NAVIGATION.md`
2. `elementor/components/FOOTER.md`

Use these files for styling and motion:

1. `elementor/custom-css/FARZAM_GLOBAL_STYLE.md`
2. `elementor/custom-js/FARZAM_PREMIUM_MOTION.md`

Use this file before writing or editing any public website copy:

1. `content/COPYWRITING_RULES.md`

---

## Copywriting Rules for Elementor

Before writing or editing any visible website text in Elementor, read:

`content/COPYWRITING_RULES.md`

All public website copy must follow these rules:

1. Do not use dashes.
2. Do not use AI-sounding language.
3. All text must feel human, natural, professional, and premium.
4. Avoid robotic sentence structures.
5. Avoid generic AI phrases.
6. Avoid over-polished artificial wording.
7. Write like a strategic human consultant.
8. Keep the tone clear, calm, executive, and trustworthy.

This rule applies to:

1. Headlines
2. Subheadlines
3. Paragraphs
4. CTAs
5. Buttons
6. Forms
7. Dashboard messages
8. Blog content
9. Course descriptions
10. SEO descriptions
11. Error messages
12. Confirmation messages
13. Newsletter copy
14. Microcopy

Important clarification:

The no-dash rule applies to public website copy and user-facing writing.

Internal documentation, Markdown files, file paths, and technical notes may use normal Markdown syntax when needed.

---

## Elementor Global Setup

Before designing pages, configure Elementor Site Settings.

### Global Colors

Use the color system from:

`elementor/custom-css/FARZAM_GLOBAL_STYLE.md`

Core colors:

1. Navy
2. Deep blue
3. White
4. Soft light background
5. Warm neutral
6. Muted gray text
7. Subtle gold accent

### Global Typography

Recommended font direction:

1. Inter
2. Manrope
3. Satoshi
4. System sans-serif fallback

Typography should feel:

1. Premium
2. Modern
3. Clean
4. Executive
5. Editorial
6. Easy to read

### Global Layout

Recommended max widths:

1. Standard container: 1180px
2. Wide container: 1320px

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

1. Logo
2. Hamburger Menu
3. Register / Sign In
4. Book a Strategy Call

Header behavior:

1. Sticky
2. Minimal
3. Light background
4. Slight blur or solid white on scroll
5. Premium spacing
6. Mobile optimized

The hamburger menu should include all main site pages.

Do not create a crowded top navigation bar.

---

## Global Footer Implementation

Use Elementor Pro Theme Builder.

Create:

`Global Footer`

Use reference:

`elementor/components/FOOTER.md`

Footer should include:

1. Brand block
2. Main navigation
3. Growth topics
4. Courses and resources
5. Newsletter signup
6. Contact CTA
7. Social links
8. Legal links

Footer should support:

1. SEO internal linking
2. Newsletter growth
3. Conversion
4. Trust

---

## Page Building Order

Build pages in this order:

1. Header
2. Footer
3. Home
4. Growth Systems
5. Modules
6. Contact
7. Blog
8. Courses
9. Studio
10. About
11. Work
12. Dashboard
13. Register
14. Login

Reason:

The header and footer define the global structure first.

The Home page then introduces the full system.

The Growth Systems and Modules pages explain the core methodology and offer structure.

The Contact page should be ready early because it carries the main conversion path.

---

## Home Page Implementation

Use:

`elementor/page-blueprints/HOME.md`

The Home page should explain:

1. Who Farzam helps
2. What Growth Systems are
3. Why scattered marketing is not enough
4. How Farzam’s approach works
5. What the visitor should do next

Hero should include:

1. Strong positioning
2. Clear CTA
3. Premium visual system
4. No generic marketing language
5. No AI-heavy positioning

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

1. What a Growth System is
2. Why businesses need one
3. How the system works
4. Why marketing and AI are only parts of the system
5. How strategy, positioning, customer journey, content, AI, and automation connect

Use diagrams, process blocks, and clean explanatory sections.

Keep language clear and human.

---

## Modules Page Implementation

Use:

`elementor/page-blueprints/MODULES.md`

This page should show Farzam’s strategic capability areas.

Each module should feel like part of a larger system, not an isolated service.

Avoid service-page clutter.

Use clean module cards.

Each module should connect to a business problem and a strategic outcome.

---

## Work Page Implementation

Use:

`elementor/page-blueprints/WORK.md`

This page should build credibility.

It should not feel like a generic portfolio gallery.

Each work item should show:

1. Context
2. Problem
3. Strategic role
4. System contribution
5. Outcome or strategic value

The Work page should prove Farzam’s ability to think strategically and execute with structure.

---

## Blog Page Implementation

Use:

`elementor/page-blueprints/BLOG.md`

The blog should support thought leadership and SEO.

Important:

SEO is not the topic of the blog.

SEO is the structure behind the blog.

Blog categories should include:

1. Growth Systems
2. Brand Positioning
3. AI Leverage
4. Customer Journey
5. Content Systems
6. Business Clarity
7. Personal Brand

Blog cards should be clean, editorial, and easy to scan.

Each blog article should connect to a strategic topic and a next action.

---

## Courses Page Implementation

Use:

`elementor/page-blueprints/COURSES.md`

The Courses page should support:

1. Free courses
2. Paid courses later
3. Webinars
4. Workshops
5. Lead magnets
6. Register / Sign In
7. YouTube audience entry
8. Skool audience entry later
9. Course-to-consulting conversion

Courses should connect education to strategic consulting.

Do not make the page feel like a cheap course marketplace.

---

## Studio Page Implementation

Use:

`elementor/page-blueprints/STUDIO.md`

This page should explain Farzam Growth Studio as the ecosystem behind the work.

It should not sound like a traditional agency.

Core idea:

System first. Marketing second. AI only when useful.

The Studio page should make the business feel structured, premium, and serious.

---

## About Page Implementation

Use:

`elementor/page-blueprints/ABOUT.md`

The About page should build credibility and human trust.

It should not be a traditional CV page.

It should explain:

1. Who Farzam is
2. How he thinks
3. His background
4. Why he builds Growth Systems
5. Why his experience is relevant
6. Why his approach is practical and business-oriented

The tone should be human, calm, and credible.

---

## Contact Page Implementation

Use:

`elementor/page-blueprints/CONTACT.md`

The Contact page should include:

1. Strategy call CTA
2. Growth Diagnosis form
3. General contact form
4. Course and webinar inquiry path
5. Collaboration inquiry path

The contact page must feel like the start of a serious strategic conversation.

Forms should feel calm, not aggressive.

---

## Dashboard Implementation

Use:

`elementor/page-blueprints/DASHBOARD.md`

The dashboard should support:

1. My Courses
2. My Webinars
3. Saved Resources
4. Growth Diagnosis Status
5. Newsletter Preferences
6. Member-only Strategy Offer
7. Account Settings

Dashboard should be noindex.

The dashboard may require a membership plugin and custom templates.

Dashboard copy must feel like a premium user hub, not a noisy account area.

---

## Register and Login Pages

Create simple, premium account pages.

### Register Page

URL:

`/register`

Purpose:

Allow users to create an account for courses, webinars, saved resources, dashboard access, and newsletter preferences.

Include:

1. Name
2. Email
3. Password
4. Consent checkbox
5. Interest category if possible

After registration, redirect to:

`/dashboard`

### Login Page

URL:

`/login`

Purpose:

Allow existing users to access their account.

After login, redirect to:

`/dashboard`

Register and login pages should be noindex.

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

1. Clean
2. Premium
3. Mobile-friendly
4. Not overwhelming
5. Connected to n8n later

For long forms, use a multi-step layout.

Form copy should follow:

`content/COPYWRITING_RULES.md`

---

## n8n Integration Direction

All important user actions should eventually connect to n8n.

Important triggers:

1. Newsletter subscription
2. Growth Diagnosis submission
3. Contact form submission
4. Course registration
5. Webinar registration
6. Strategy call booking
7. Dashboard activity
8. Resource download
9. Member offer click

n8n should support:

1. Email confirmation
2. Lead segmentation
3. CRM updates
4. Follow-up sequences
5. Course-to-consulting conversion
6. Newsletter preference management

Automation should not make the brand feel robotic.

---

## SEO Implementation

Use:

`seo/SEO_ARCHITECTURE.md`

For each page:

1. One clear H1
2. Clean URL slug
3. SEO title
4. Meta description
5. Internal links
6. Structured headings
7. Topic consistency
8. No keyword stuffing

Important:

Dashboard, login, register, and account pages should usually be noindex.

Blog posts should be SEO structured.

SEO descriptions must also follow:

`content/COPYWRITING_RULES.md`

---

## Design System Implementation

Use:

`design-system/DESIGN_SYSTEM.md`

Visual style should be:

1. Premium
2. Minimal
3. Executive
4. Spacious
5. White and light
6. Strategic
7. Calm
8. Trustworthy

Avoid:

1. Noisy gradients
2. Generic stock images
3. Heavy AI visuals
4. Loud agency graphics
5. Dark tech cliché design
6. Cheap icon systems
7. Overdesigned effects

---

## Motion Implementation

Use:

`elementor/custom-js/FARZAM_PREMIUM_MOTION.md`

Apply motion carefully.

Recommended classes:

1. `fgs-reveal`
2. `fgs-stagger`
3. `fgs-card`
4. `fgs-btn-primary`
5. `fgs-btn-secondary`

Motion must be:

1. Calm
2. Subtle
3. Lightweight
4. Accessible
5. Non-distracting

Avoid:

1. Heavy parallax
2. Scroll hijacking
3. Loud transitions
4. Neon effects
5. AI particles
6. Bouncy animations

---

## Mobile Implementation

Every page must be mobile optimized.

Mobile priorities:

1. Clear hero
2. Readable typography
3. Large tap targets
4. Simple navigation
5. Clean forms
6. No overcrowded sections
7. Fast loading
8. Dashboard usability
9. No horizontal scroll

The mobile experience should feel as premium as desktop.

---

## Performance Requirements

Keep the website fast.

Avoid:

1. Heavy animation libraries
2. Too many plugins
3. Large uncompressed images
4. Unnecessary sliders
5. Auto-playing videos
6. Excessive custom code
7. Overbuilt Elementor sections

Use:

1. Optimized images
2. Lightweight CSS
3. Minimal JavaScript
4. Lazy loading
5. Clean Elementor structure
6. Caching
7. Good hosting configuration

---

## Accessibility Requirements

Website should include:

1. Good color contrast
2. Keyboard accessible navigation
3. Clear focus states
4. Form labels
5. Accessible buttons
6. Proper heading hierarchy
7. Reduced motion support
8. Clear link text

Accessibility should support the premium feel, not be treated as a separate checklist only.

---

## Elementor Class Usage

Use consistent classes across pages.

Recommended classes:

1. `fgs-section`
2. `fgs-section-compact`
3. `fgs-section-soft`
4. `fgs-container`
5. `fgs-container-wide`
6. `fgs-card`
7. `fgs-module-card`
8. `fgs-blog-card`
9. `fgs-course-card`
10. `fgs-btn-primary`
11. `fgs-btn-secondary`
12. `fgs-reveal`
13. `fgs-stagger`
14. `fgs-form`
15. `fgs-dashboard-card`

Do not create random one-off class names unless necessary.

---

## Elementor Section Quality Rules

Every Elementor section should have:

1. Clear purpose
2. Clean spacing
3. Strong hierarchy
4. One main message
5. Clear next action if needed

Avoid:

1. Too many columns
2. Too many widgets
3. Unclear visual priority
4. Random icons
5. Repeated CTA clutter
6. Long text blocks without structure

---

## Public Copy QA Before Publishing

Before publishing any public website copy, check:

1. Does it sound human?
2. Does it sound like Farzam?
3. Does it avoid dashes?
4. Does it avoid AI-sounding phrasing?
5. Does it avoid hype?
6. Does it support Growth System positioning?
7. Does it avoid freelancer or agency positioning?
8. Is the sentence useful?
9. Is the next step clear?
10. Would a serious business audience trust this?

If the answer is no, rewrite it.

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

A premium strategic platform built around Farzam’s thinking, methodology, education, consulting path, and automation infrastructure.
