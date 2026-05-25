# WordPress and Elementor Build Tasks

## Purpose

This document defines the practical build tasks for implementing Farzam.nl in WordPress and Elementor Pro.

It translates the strategy, sitemap, design system, page blueprints, SEO architecture, and automation plan into an execution checklist.

The goal is to build Farzam.nl as a premium Growth System platform, not as a generic portfolio, agency website, or AI landing page.

---

## Core Build Principle

Every task should support the main positioning:

Build a Growth System, not just more marketing.

The website must position Farzam as:

- Growth Strategist
- Growth System Designer
- Business-Oriented Thinker

The website must avoid positioning him as:

- Traditional marketer
- Freelance marketer
- Social media manager
- AI tool operator
- Generic agency owner

---

## Phase 1: WordPress Foundation

### Task 1: Confirm WordPress Installation

Check that WordPress is installed and accessible.

Required:

- Admin access works
- SSL is active
- Website loads correctly
- Permalinks are set to clean URLs

Recommended permalink structure:

`/%postname%/`

---

### Task 2: Install Required Plugins

Install core plugins first.

Required for MVP:

- Elementor
- Elementor Pro
- Yoast SEO
- Code Snippets or equivalent custom code tool
- Form plugin if Elementor forms are not enough
- Security plugin
- Backup plugin
- Cache / performance plugin

Recommended later:

- Ultimate Member or ProfilePress
- Tutor LMS or LearnDash
- FluentBooking or Calendly embed
- WooCommerce if paid courses are needed later

---

### Task 3: Configure Basic WordPress Settings

Set:

- Site title: Farzam Gholizadeh
- Tagline: Growth Strategist and Growth System Designer
- Timezone: Netherlands
- Language: English
- Homepage: static Home page later
- Blog page: Blog later

---

## Phase 2: Elementor Global Setup

### Task 4: Configure Elementor Site Settings

Use:

`elementor/custom-css/FARZAM_GLOBAL_STYLE.md`

Set:

- Global colors
- Global fonts
- Button styles
- Container width
- Typography hierarchy
- Form styling direction

Recommended style:

- Premium
- Minimal
- Executive
- Spacious
- Clean
- Light

---

### Task 5: Add Global Custom CSS

Add global CSS through one of these methods:

- Elementor Site Settings Custom CSS
- WordPress Customizer Additional CSS
- Code Snippets
- Child theme stylesheet later

Use the CSS direction from:

`elementor/custom-css/FARZAM_GLOBAL_STYLE.md`

---

### Task 6: Add Premium Motion JavaScript

Use:

`elementor/custom-js/FARZAM_PREMIUM_MOTION.md`

Add JavaScript through:

- Elementor Custom Code
- Code Snippets
- Child theme later

Use only lightweight motion.

Motion should be:

- Calm
- Subtle
- Premium
- Accessible
- Non-distracting

---

## Phase 3: Global Components

### Task 7: Build Global Header

Use Elementor Pro Theme Builder.

Reference:

`elementor/components/HEADER_NAVIGATION.md`

Visible header items:

- Logo
- Hamburger Menu
- Register / Sign In
- Book a Strategy Call

Header behavior:

- Sticky
- Minimal
- Light background
- Premium spacing
- Mobile optimized

Hamburger menu includes:

- Home
- Growth Systems
- Modules
- Work
- Blog
- Courses
- Studio
- About
- Contact
- Register
- Sign In
- Dashboard

---

### Task 8: Build Global Footer

Use Elementor Pro Theme Builder.

Reference:

`elementor/components/FOOTER.md`

Footer must include:

- Brand block
- Main navigation
- Growth topics
- Courses and resources
- Newsletter signup
- Contact CTA
- Social links
- Legal links

Footer should support:

- SEO
- Trust
- Newsletter growth
- Conversion

---

## Phase 4: Create WordPress Pages

### Task 9: Create Main Pages

Create these pages in WordPress:

1. Home
2. Growth Systems
3. Modules
4. Work
5. Blog
6. Courses
7. Studio
8. About
9. Contact
10. Dashboard
11. Register
12. Login

Set slugs:

- `/`
- `/growth-systems`
- `/modules`
- `/work`
- `/blog`
- `/courses`
- `/studio`
- `/about`
- `/contact`
- `/dashboard`
- `/register`
- `/login`

---

### Task 10: Set Home and Blog Pages

In WordPress settings:

Set homepage to:

`Home`

Set posts page to:

`Blog`

---

## Phase 5: Page Build Priority

Build pages in this exact order.

### Priority 1: Home

Reference:

`elementor/page-blueprints/HOME.md`

Goal:

Explain the full positioning and direct users toward Growth Systems or Strategy Call.

---

### Priority 2: Growth Systems

Reference:

`elementor/page-blueprints/GROWTH_SYSTEMS.md`

Goal:

Explain Farzam’s core methodology.

This is one of the most important pages.

---

### Priority 3: Modules

Reference:

`elementor/page-blueprints/MODULES.md`

Goal:

Show strategic capability areas without making the page feel like a generic services page.

---

### Priority 4: Contact

Reference:

`elementor/page-blueprints/CONTACT.md`

Goal:

Convert visitors into Growth Diagnosis submissions, strategy calls, and qualified inquiries.

---

### Priority 5: Blog

Reference:

`elementor/page-blueprints/BLOG.md`

Goal:

Build thought leadership and organic SEO structure.

---

### Priority 6: Courses

Reference:

`elementor/page-blueprints/COURSES.md`

Goal:

Prepare the education, webinar, lead magnet, and course-to-consulting system.

---

### Priority 7: Studio

Reference:

`elementor/page-blueprints/STUDIO.md`

Goal:

Explain Farzam Growth Studio as the ecosystem behind the work.

---

### Priority 8: About

Reference:

`elementor/page-blueprints/ABOUT.md`

Goal:

Build human trust and professional credibility.

---

### Priority 9: Work

Reference:

`elementor/page-blueprints/WORK.md`

Goal:

Show selected experience and strategic proof.

---

### Priority 10: Dashboard

Reference:

`elementor/page-blueprints/DASHBOARD.md`

Goal:

Create a premium user account experience.

This may require membership plugin setup.

---

## Phase 6: Forms and Conversion System

### Task 11: Build Growth Diagnosis Form

Place mainly on:

`/contact`

Possible additional placement:

- Home CTA
- Growth Systems CTA
- Dashboard

Recommended fields:

- Name
- Email
- Company / project
- Website
- Business type
- Current growth challenge
- Where growth feels broken
- Main priority
- Marketing maturity
- AI / automation usage
- Budget range
- Desired outcome
- Preferred collaboration type
- Message

CTA:

Submit Growth Diagnosis

---

### Task 12: Build Contact Form

Place on:

`/contact`

Fields:

- Name
- Email
- Company / project
- Website
- Inquiry type
- Message
- Consent checkbox

Inquiry types:

- Strategy call
- Growth Diagnosis
- Course or webinar
- Collaboration
- Speaking / workshop
- Other

---

### Task 13: Build Newsletter Form

Place in:

- Footer
- Blog
- Courses
- Home if needed

Fields:

- Name
- Email
- Interest category
- Consent checkbox

Interest categories:

- Growth Systems
- Brand Positioning
- AI Leverage
- Customer Journey
- Content Systems
- Business Clarity
- Personal Brand
- Courses and Webinars

---

### Task 14: Build Strategy Call Booking

Use one of:

- Calendly embed
- FluentBooking
- Amelia

Place on:

- Contact page
- Header CTA
- Dashboard
- Final CTAs on key pages

---

## Phase 7: Account System

### Task 15: Set Up Register Page

URL:

`/register`

Purpose:

Allow users to create an account for:

- Courses
- Webinars
- Saved resources
- Dashboard
- Newsletter preferences
- Member-only strategy offers

Required fields:

- Name
- Email
- Password
- Consent checkbox

After registration:

Redirect to:

`/dashboard`

---

### Task 16: Set Up Login Page

URL:

`/login`

Purpose:

Allow users to access their dashboard.

After login:

Redirect to:

`/dashboard`

---

### Task 17: Build Dashboard

Reference:

`elementor/page-blueprints/DASHBOARD.md`

Dashboard sections:

- Overview
- My Courses
- My Webinars
- Saved Resources
- Growth Diagnosis Status
- Newsletter Preferences
- Member-only Strategy Offer
- Account Settings

SEO setting:

Noindex

---

## Phase 8: SEO Setup

### Task 18: Configure Yoast SEO

Use:

`seo/SEO_ARCHITECTURE.md`

For each page:

- SEO title
- Meta description
- Slug
- One H1
- Clean heading hierarchy
- Internal links
- Focus topic
- Schema if useful

Noindex:

- Dashboard
- Register
- Login
- Account pages
- Thank-you pages

---

### Task 19: Blog Category Structure

Create blog categories:

- Growth Systems
- Brand Positioning
- AI Leverage
- Customer Journey
- Content Systems
- Business Clarity
- Personal Brand

Important:

SEO is the architecture behind the blog.

SEO is not the blog topic itself.

---

### Task 20: Internal Linking

Add internal links across pages.

Priority links:

- Home to Growth Systems
- Home to Modules
- Home to Contact
- Growth Systems to Modules
- Modules to Contact
- Blog to Growth Systems
- Courses to Dashboard
- Studio to Contact
- About to Work and Studio
- Footer to all key pages

---

## Phase 9: n8n Automation Preparation

### Task 21: Prepare Automation Events

Reference:

`n8n/AUTOMATION_ARCHITECTURE.md`

Track these events:

- Newsletter subscription
- Contact form submission
- Growth Diagnosis submission
- Strategy call booking
- Course registration
- Webinar registration
- Resource download
- Dashboard activity
- Member offer click

---

### Task 22: Define Data Fields

Capture:

- Name
- Email
- Company
- Website
- Source page
- CTA clicked
- Interest category
- Growth challenge
- Inquiry type
- UTM source
- UTM campaign
- Consent
- Timestamp

---

### Task 23: Connect Forms to n8n Later

MVP can start with email notifications.

Later connect forms to:

- n8n webhook
- CRM
- Google Sheets
- Email sequence
- Lead segmentation
- Dashboard status update

---

## Phase 10: Content and Visual QA

### Task 24: Copy Quality Check

Every page must avoid:

- Robotic wording
- AI clichés
- Generic agency language
- Overhyped AI claims
- Social media manager positioning
- Freelancer-style copy

Every page must feel:

- Human
- Strategic
- Premium
- Clear
- Confident
- Business-oriented

---

### Task 25: Design Quality Check

Every page must feel:

- Spacious
- Minimal
- Premium
- Executive
- Clean
- Calm
- System-oriented

Avoid:

- Crowded sections
- Generic stock images
- Heavy gradients
- Loud animation
- Cheap icons
- Template-heavy layout

---

### Task 26: Mobile QA

Check every page on mobile.

Required:

- Header works
- Hamburger works
- CTA visible
- Text readable
- Forms usable
- Cards stack cleanly
- Footer not too long or messy
- No horizontal scroll

---

### Task 27: Performance QA

Check:

- Image size
- Plugin load
- CSS size
- JavaScript load
- Mobile speed
- Elementor section complexity
- Cache plugin setup

Avoid:

- Heavy sliders
- Auto-playing videos
- Too many effects
- Too many plugins
- Large uncompressed images

---

### Task 28: Accessibility QA

Check:

- Heading hierarchy
- Button labels
- Link clarity
- Form labels
- Color contrast
- Keyboard navigation
- Reduced motion behavior

---

## Phase 11: Launch Preparation

### Task 29: Legal Pages

Create:

- Privacy Policy
- Terms of Use
- Cookie Policy if needed

Important because the site collects:

- Newsletter subscriptions
- Contact form data
- User registration data
- Course / webinar interest
- Dashboard activity later

---

### Task 30: Final Launch Checklist

Before launch:

- All key pages published
- Header and footer active
- Forms tested
- Booking tested
- SEO titles and meta descriptions added
- Mobile checked
- Speed checked
- Links checked
- Dashboard noindexed
- Login/register tested
- Newsletter form tested
- Analytics added if needed
- Backup configured

---

## MVP Scope

For MVP, focus on:

1. Home
2. Growth Systems
3. Modules
4. Contact
5. Blog structure
6. Header
7. Footer
8. Basic newsletter
9. Growth Diagnosis form
10. Strategy Call CTA

Dashboard, courses, full automation, and advanced membership can be Phase 2.

---

## Phase 2 Scope

After MVP:

- Courses
- Webinars
- Dashboard
- Account system
- Saved resources
- Member-only offers
- n8n CRM workflows
- Course-to-consulting automation
- Advanced SEO blog system
- YouTube / Skool integration

---

## Final Build Rule

Do not build random pages.

Do not add features because they are trendy.

Do not make the site look like an agency template.

Every build decision must support one system:

Visitor  
→ Understand  
→ Trust  
→ Learn  
→ Register  
→ Diagnose  
→ Book  
→ Convert

Farzam.nl is the digital Growth System behind Farzam’s personal brand and consulting ecosystem.
