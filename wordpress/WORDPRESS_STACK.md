# Farzam.nl WordPress Stack

## Purpose

This document defines the recommended WordPress stack for Farzam.nl.

Farzam.nl will be built on WordPress with Elementor Pro and should support:

- Premium personal brand website
- Growth System consultancy positioning
- Blog content engine
- Courses and webinars
- Register / Sign In
- User dashboard
- Newsletter growth
- Lead capture
- Strategy call booking
- n8n automation
- SEO structure across all pages

The goal is to keep the first version practical, fast, premium, and scalable.

---

## Core Platform

### WordPress

WordPress will be the main CMS and website platform.

Use WordPress for:
- Main pages
- Blog
- Courses landing pages
- User registration foundation
- Forms
- SEO structure
- Content publishing
- Elementor templates

---

## Page Builder

### Elementor Pro

Elementor Pro should be the primary design and page-building system.

Use Elementor Pro for:
- Header
- Footer
- Page templates
- Landing pages
- Blog templates
- Course landing pages
- CTA sections
- Forms if suitable
- Motion and interactions
- Reusable design components

Important rules:
- Use global colors
- Use global typography
- Use reusable templates
- Keep containers clean
- Avoid too many nested sections
- Keep pages fast and responsive

---

## SEO

### Yoast SEO

Yoast SEO should be used for:
- Meta titles
- Meta descriptions
- XML sitemap
- Canonical URLs
- Breadcrumbs if needed
- Basic schema support
- SEO readability checks

SEO principle:
SEO must be applied across all pages, not only the blog.

Every page should have:
- One H1
- Clear H2/H3 hierarchy
- Keyword intent
- Internal links
- Optimized metadata
- Structured content
- Conversion CTA

---

## Forms

Recommended options:

### Preferred MVP Option: Fluent Forms

Use Fluent Forms for:
- Contact form
- Growth Diagnosis form
- Newsletter signup
- Course interest forms
- Webinar registration forms
- Lead magnet forms

Why:
- Flexible forms
- Webhook support
- Good integration options
- Easier connection to n8n

### Alternative: Gravity Forms

Use Gravity Forms if more advanced conditional logic is required.

---

## n8n Integration

Recommended connection methods:

### Option 1: Fluent Forms Webhooks

Best for:
- Form submissions
- Growth Diagnosis form
- Newsletter signup
- Course/webinar interest forms

### Option 2: WP Webhooks

Use if deeper WordPress events need to trigger n8n.

Possible triggers:
- User registered
- Course enrolled
- WooCommerce purchase
- Form submitted
- Post published

### Option 3: WooCommerce Webhooks

Use for:
- Course purchase
- Product purchase
- Payment completed
- Order status changed

---

## User Registration and Account System

Farzam.nl should support:

- Register / Sign In
- Profile / Dashboard
- My Courses
- My Webinars
- Saved Resources
- Newsletter Preferences
- Member-only Strategy Offer

### MVP Option

Use a lightweight member/account plugin first.

Recommended plugins:
- Ultimate Member
- ProfilePress
- Paid Memberships Pro if membership access becomes important

MVP goal:
Create a simple account system without overcomplicating the first launch.

### Advanced Option

Later, use a more complete membership stack if needed:
- Paid Memberships Pro
- WooCommerce Memberships
- MemberPress

---

## Courses and Webinars

The Courses section should support:
- Free courses
- Paid courses
- Workshops
- Webinars
- YouTube audience entry
- Skool audience entry
- Course-to-consulting conversion

### MVP Course Strategy

For the first version:
- Use Courses as a premium landing page
- Offer free resources, webinars, and waitlists
- Use registration forms to capture leads
- Connect everything to n8n
- Keep actual course delivery simple

Recommended MVP setup:
- Elementor course landing pages
- Fluent Forms for registration
- WooCommerce only if paid access is needed immediately
- External delivery through Skool, YouTube private links, Zoom, or manual email if needed

### Full LMS Option

When ready to scale, consider:
- Tutor LMS
- LearnDash
- LifterLMS
- Sensei LMS

Best fit later:
Tutor LMS or LearnDash.

Use LMS when:
- Courses need lessons
- Progress tracking is needed
- Paid course access is required
- User dashboard must show course progress
- Certificates or quizzes are needed

---

## WooCommerce

WooCommerce is already available and can support:
- Paid courses
- Paid workshops
- Consulting session products
- Digital downloads
- Coupon codes
- Member offers

For MVP:
Do not make WooCommerce the center of the site unless paid offers are ready.

Use WooCommerce later for:
- Course payments
- Webinar payments
- Consulting package payments
- Member-only offers
- Discount codes

---

## Booking System

The website needs a premium booking path for strategy calls.

Options:

### Option 1: Calendly Embed

Best for MVP.

Pros:
- Fast setup
- Reliable
- Easy user experience
- Can connect to n8n via webhook or Zapier/n8n integration

### Option 2: FluentBooking

Good WordPress-native option.

Pros:
- Native WordPress experience
- Can connect with Fluent ecosystem
- Good for booking forms and calendar control

### Option 3: Amelia

Good for more advanced booking needs.

Pros:
- Professional booking interface
- Services, appointments, payments
- Good for consulting workflows

Recommended MVP:
Calendly or FluentBooking.

Primary CTA:
Book a Strategy Call

---

## Email Marketing

Possible tools:

### FluentCRM

Good if keeping email marketing inside WordPress.

Pros:
- WordPress-native
- Works well with Fluent Forms
- Can segment users
- Can support simple automation

### Brevo

Good external email marketing option.

Pros:
- Affordable
- Strong email deliverability
- Good automation
- Works with n8n

### Mailchimp

Possible but less preferred for this system.

Recommended:
Brevo or FluentCRM.

For a more scalable setup:
Use Brevo + n8n.

---

## CRM

For MVP, CRM can start simple.

Options:
- Airtable
- Notion
- Google Sheets
- HubSpot CRM
- FluentCRM
- Brevo CRM features

Recommended MVP:
Airtable or HubSpot CRM connected through n8n.

CRM stages:
1. New Lead
2. Newsletter Subscriber
3. Registered User
4. Course / Webinar Lead
5. Growth Diagnosis Completed
6. Strategy Call Booked
7. Call Completed
8. Proposal Needed
9. Proposal Sent
10. Client
11. Long-Term Nurture

---

## Blog System

Use WordPress native posts.

Blog categories:
- Growth Systems
- Brand Positioning
- AI Leverage
- Customer Journey
- Content Systems
- Business Clarity
- Personal Brand

Blog requirements:
- SEO-structured articles
- Category archives
- Internal links
- Newsletter CTA
- Related articles
- Social repurposing workflow
- n8n trigger when new post is published

---

## Security and Performance

Recommended plugins or features:
- Wordfence Security or Solid Security
- LiteSpeed Cache or WP Rocket
- ShortPixel or Imagify for image compression
- UpdraftPlus for backups
- Cloudflare if available

Performance rules:
- Avoid unnecessary plugins
- Use WebP images
- Compress images
- Lazy load visuals
- Keep Elementor sections lightweight
- Avoid heavy animation libraries
- Test mobile speed

---

## Analytics and Tracking

Use:
- Google Analytics 4
- Google Search Console
- Microsoft Clarity or Hotjar if needed
- n8n lead source tracking
- UTM tracking
- Conversion tracking for forms and booking

Track:
- Newsletter signups
- Growth Diagnosis submissions
- Course registrations
- Webinar registrations
- Strategy call bookings
- Blog-to-lead conversion
- Source attribution

---

## Recommended MVP Plugin Stack

For launch-ready MVP:

1. Elementor Pro
2. Yoast SEO
3. Fluent Forms
4. FluentBooking or Calendly embed
5. Brevo or FluentCRM
6. WP Webhooks
7. WooCommerce installed but not central yet
8. LiteSpeed Cache or WP Rocket
9. ShortPixel or Imagify
10. Wordfence or Solid Security
11. UpdraftPlus

Optional later:
- Tutor LMS or LearnDash
- Paid Memberships Pro
- WooCommerce Memberships
- Amelia
- HubSpot integration

---

## MVP Build Strategy

Phase 1 should focus on:
- Premium website structure
- Home
- Growth Systems
- Modules
- Work
- Blog
- Courses landing
- Studio
- About
- Contact
- Newsletter signup
- Growth Diagnosis form
- Strategy call booking
- n8n-ready form structure

Phase 2 should add:
- Register / Sign In
- Basic user dashboard
- My Courses
- My Webinars
- Saved Resources
- Newsletter Preferences
- Member-only Strategy Offer

Phase 3 should add:
- Paid courses
- Webinars
- WooCommerce payments
- LMS integration
- Advanced segmentation
- Full email nurture automation

Phase 4 should optimize:
- CRM pipeline
- Lead scoring
- SEO growth
- Content repurposing
- Paid offers
- Conversion rates

---

## Final Recommendation

Do not overbuild the first version.

Launch Farzam.nl first as a premium Growth Platform MVP.

Build:
- Strong positioning
- Clear sitemap
- SEO structure
- Blog engine
- Courses entry point
- Lead capture
- Booking path
- n8n automation readiness

Then scale into:
- Full dashboard
- Paid courses
- Webinars
- Membership
- Advanced CRM
- Automated content and sales systems
