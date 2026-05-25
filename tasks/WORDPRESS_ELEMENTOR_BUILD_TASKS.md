# WordPress and Elementor Build Tasks

## Purpose

This document defines the practical build tasks for implementing Farzam.nl in WordPress and Elementor Pro.

It translates the strategy, sitemap, design system, page blueprints, SEO architecture, copywriting rules, and automation plan into an execution checklist.

The goal is to build Farzam.nl as a premium Growth System platform, not as a generic portfolio, agency website, or AI landing page.

---

## Core Build Principle

Every task should support the main positioning:

Build a Growth System, not just more marketing.

The website must position Farzam as:

1. Growth Strategist
2. Growth System Designer
3. Business-Oriented Thinker

The website must avoid positioning him as:

1. Traditional marketer
2. Freelance marketer
3. Social media manager
4. AI tool operator
5. Generic agency owner

Marketing, content, AI, automation, websites, and campaigns are tools inside the Growth System.

They are not the identity of the brand.

---

## Required Reading Before Build

Before starting implementation, read these files in order:

1. `README.md`
2. `AGENTS.md`
3. `PROJECT_BRIEF.md`
4. `content/COPYWRITING_RULES.md`
5. `elementor/ELEMENTOR_IMPLEMENTATION_GUIDE.md`
6. `design-system/DESIGN_SYSTEM.md`
7. `seo/SEO_ARCHITECTURE.md`
8. `wordpress/WORDPRESS_STACK.md`
9. `n8n/AUTOMATION_ARCHITECTURE.md`

Before writing or editing any public website copy, always read:

`content/COPYWRITING_RULES.md`

---

## Public Copywriting Rule

All public website copy must follow these rules:

1. Do not use dashes.
2. Do not use AI-sounding language.
3. All text must feel human, natural, professional, and premium.
4. Avoid robotic sentence structures.
5. Avoid generic AI phrases.
6. Avoid over-polished artificial wording.
7. Write like a strategic human consultant.
8. Keep the tone clear, calm, executive, and trustworthy.

This applies to:

1. Page copy
2. Headlines
3. Subheadlines
4. CTAs
5. Button labels
6. Form text
7. Blog content
8. Course descriptions
9. Dashboard messages
10. Email copy
11. Newsletter copy
12. SEO descriptions
13. Microcopy
14. Error messages
15. Confirmation messages

Important clarification:

The no-dash rule applies to public website copy and user-facing writing.

Markdown documentation files may use normal Markdown syntax when needed for structure, lists, file paths, and technical notes.

---

## Phase 1: WordPress Foundation

### Task 1: Confirm WordPress Installation

Check that WordPress is installed and accessible.

Required:

1. Admin access works
2. SSL is active
3. Website loads correctly
4. Permalinks are set to clean URLs
5. WordPress dashboard is accessible
6. Theme and plugin area is accessible

Recommended permalink structure:

`/%postname%/`

---

### Task 2: Install Required Plugins

Install core plugins first.

Required for MVP:

1. Elementor
2. Elementor Pro
3. Yoast SEO
4. Code Snippets or equivalent custom code tool
5. Form plugin if Elementor forms are not enough
6. Security plugin
7. Backup plugin
8. Cache or performance plugin

Recommended later:

1. Ultimate Member or ProfilePress
2. Tutor LMS or LearnDash
3. FluentBooking or Calendly embed
4. WooCommerce if paid courses are needed later
5. Newsletter or CRM integration plugin if needed

Avoid installing too many plugins at the beginning.

Keep the setup clean and lightweight.

---

### Task 3: Configure Basic WordPress Settings

Set:

1. Site title: Farzam Gholizadeh
2. Tagline: Growth Strategist and Growth System Designer
3. Timezone: Netherlands
4. Language: English
5. Homepage: static Home page later
6. Blog page: Blog later

Also check:

1. Site visibility settings
2. User registration settings
3. Media upload settings
4. Permalink structure
5. Comment settings

---

## Phase 2: Elementor Global Setup

### Task 4: Configure Elementor Site Settings

Use:

`elementor/custom-css/FARZAM_GLOBAL_STYLE.md`

Set:

1. Global colors
2. Global fonts
3. Button styles
4. Container width
5. Typography hierarchy
6. Form styling direction
7. Section spacing direction
8. Responsive breakpoints if needed

Recommended style:

1. Premium
2. Minimal
3. Executive
4. Spacious
5. Clean
6. Light
7. Calm
8. System-oriented

---

### Task 5: Add Global Custom CSS

Add global CSS through one of these methods:

1. Elementor Site Settings Custom CSS
2. WordPress Customizer Additional CSS
3. Code Snippets
4. Child theme stylesheet later

Use the CSS direction from:

`elementor/custom-css/FARZAM_GLOBAL_STYLE.md`

Do not add random one-off styles unless necessary.

Use consistent class names.

---

### Task 6: Add Premium Motion JavaScript

Use:

`elementor/custom-js/FARZAM_PREMIUM_MOTION.md`

Add JavaScript through:

1. Elementor Custom Code
2. Code Snippets
3. Child theme later

Use only lightweight motion.

Motion should be:

1. Calm
2. Subtle
3. Premium
4. Accessible
5. Non-distracting

Avoid:

1. Heavy parallax
2. Neon effects
3. Bouncy animation
4. AI particles
5. Scroll hijacking
6. Auto-moving sliders

---

## Phase 3: Global Components

### Task 7: Build Global Header

Use Elementor Pro Theme Builder.

Reference:

`elementor/components/HEADER_NAVIGATION.md`

Visible header items:

1. Logo
2. Hamburger Menu
3. Register / Sign In
4. Book a Strategy Call

Header behavior:

1. Sticky
2. Minimal
3. Light background
4. Premium spacing
5. Mobile optimized
6. Slight scroll state if needed

Hamburger menu includes:

1. Home
2. Growth Systems
3. Modules
4. Work
5. Blog
6. Courses
7. Studio
8. About
9. Contact
10. Register
11. Sign In
12. Dashboard

Do not create a crowded top navigation bar.

---

### Task 8: Build Global Footer

Use Elementor Pro Theme Builder.

Reference:

`elementor/components/FOOTER.md`

Footer must include:

1. Brand block
2. Main navigation
3. Growth topics
4. Courses and resources
5. Newsletter signup
6. Contact CTA
7. Social links
8. Legal links

Footer should support:

1. SEO
2. Trust
3. Newsletter growth
4. Conversion
5. Internal linking

Footer must remain calm, structured, and premium.

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

1. `/`
2. `/growth-systems`
3. `/modules`
4. `/work`
5. `/blog`
6. `/courses`
7. `/studio`
8. `/about`
9. `/contact`
10. `/dashboard`
11. `/register`
12. `/login`

---

### Task 10: Set Home and Blog Pages

In WordPress settings:

Set homepage to:

`Home`

Set posts page to:

`Blog`

Make sure the Blog page supports future article publishing and category structure.

---

## Phase 5: Page Build Priority

Build pages in this exact order.

### Priority 1: Home

Reference:

`elementor/page-blueprints/HOME.md`

Goal:

Explain the full positioning and direct users toward Growth Systems or Strategy Call.

Before writing visible copy, check:

`content/COPYWRITING_RULES.md`

---

### Priority 2: Growth Systems

Reference:

`elementor/page-blueprints/GROWTH_SYSTEMS.md`

Goal:

Explain Farzam’s core methodology.

This is one of the most important pages.

The page must explain Growth Systems clearly and avoid sounding like a marketing service page.

Before writing visible copy, check:

`content/COPYWRITING_RULES.md`

---

### Priority 3: Modules

Reference:

`elementor/page-blueprints/MODULES.md`

Goal:

Show strategic capability areas without making the page feel like a generic services page.

Before writing visible copy, check:

`content/COPYWRITING_RULES.md`

---

### Priority 4: Contact

Reference:

`elementor/page-blueprints/CONTACT.md`

Goal:

Convert visitors into Growth Diagnosis submissions, strategy calls, and qualified inquiries.

Before writing visible copy, check:

`content/COPYWRITING_RULES.md`

---

### Priority 5: Blog

Reference:

`elementor/page-blueprints/BLOG.md`

Goal:

Build thought leadership and organic SEO structure.

Before writing visible copy, check:

`content/COPYWRITING_RULES.md`

---

### Priority 6: Courses

Reference:

`elementor/page-blueprints/COURSES.md`

Goal:

Prepare the education, webinar, lead magnet, and course-to-consulting system.

Before writing visible copy, check:

`content/COPYWRITING_RULES.md`

---

### Priority 7: Studio

Reference:

`elementor/page-blueprints/STUDIO.md`

Goal:

Explain Farzam Growth Studio as the ecosystem behind the work.

Before writing visible copy, check:

`content/COPYWRITING_RULES.md`

---

### Priority 8: About

Reference:

`elementor/page-blueprints/ABOUT.md`

Goal:

Build human trust and professional credibility.

Before writing visible copy, check:

`content/COPYWRITING_RULES.md`

---

### Priority 9: Work

Reference:

`elementor/page-blueprints/WORK.md`

Goal:

Show selected experience and strategic proof.

Before writing visible copy, check:

`content/COPYWRITING_RULES.md`

---

### Priority 10: Dashboard

Reference:

`elementor/page-blueprints/DASHBOARD.md`

Goal:

Create a premium user account experience.

This may require membership plugin setup.

Dashboard should be noindex.

Before writing visible copy, check:

`content/COPYWRITING_RULES.md`

---

## Phase 6: Forms and Conversion System

### Task 11: Build Growth Diagnosis Form

Place mainly on:

`/contact`

Possible additional placement:

1. Home CTA
2. Growth Systems CTA
3. Dashboard

Recommended fields:

1. Name
2. Email
3. Company or project
4. Website
5. Business type
6. Current growth challenge
7. Where growth feels broken
8. Main priority
9. Marketing maturity
10. AI or automation usage
11. Budget range
12. Desired outcome
13. Preferred collaboration type
14. Message

CTA:

Submit Growth Diagnosis

Form copy must follow:

`content/COPYWRITING_RULES.md`

---

### Task 12: Build Contact Form

Place on:

`/contact`

Fields:

1. Name
2. Email
3. Company or project
4. Website
5. Inquiry type
6. Message
7. Consent checkbox

Inquiry types:

1. Strategy call
2. Growth Diagnosis
3. Course or webinar
4. Collaboration
5. Speaking or workshop
6. Other

Form copy must follow:

`content/COPYWRITING_RULES.md`

---

### Task 13: Build Newsletter Form

Place in:

1. Footer
2. Blog
3. Courses
4. Home if needed

Fields:

1. Name
2. Email
3. Interest category
4. Consent checkbox

Interest categories:

1. Growth Systems
2. Brand Positioning
3. AI Leverage
4. Customer Journey
5. Content Systems
6. Business Clarity
7. Personal Brand
8. Courses and Webinars

Newsletter copy must follow:

`content/COPYWRITING_RULES.md`

---

### Task 14: Build Strategy Call Booking

Use one of:

1. Calendly embed
2. FluentBooking
3. Amelia

Place on:

1. Contact page
2. Header CTA
3. Dashboard
4. Final CTAs on key pages

Booking copy must feel calm, premium, and serious.

It must follow:

`content/COPYWRITING_RULES.md`

---

## Phase 7: Account System

### Task 15: Set Up Register Page

URL:

`/register`

Purpose:

Allow users to create an account for:

1. Courses
2. Webinars
3. Saved resources
4. Dashboard
5. Newsletter preferences
6. Member-only strategy offers

Required fields:

1. Name
2. Email
3. Password
4. Consent checkbox

After registration:

Redirect to:

`/dashboard`

Register page should be noindex.

Visible copy must follow:

`content/COPYWRITING_RULES.md`

---

### Task 16: Set Up Login Page

URL:

`/login`

Purpose:

Allow users to access their dashboard.

After login:

Redirect to:

`/dashboard`

Login page should be noindex.

Visible copy must follow:

`content/COPYWRITING_RULES.md`

---

### Task 17: Build Dashboard

Reference:

`elementor/page-blueprints/DASHBOARD.md`

Dashboard sections:

1. Overview
2. My Courses
3. My Webinars
4. Saved Resources
5. Growth Diagnosis Status
6. Newsletter Preferences
7. Member-only Strategy Offer
8. Account Settings

SEO setting:

Noindex

Dashboard copy must follow:

`content/COPYWRITING_RULES.md`

---

## Phase 8: SEO Setup

### Task 18: Configure Yoast SEO

Use:

`seo/SEO_ARCHITECTURE.md`

For each page:

1. SEO title
2. Meta description
3. Slug
4. One H1
5. Clean heading hierarchy
6. Internal links
7. Focus topic
8. Schema if useful

Noindex:

1. Dashboard
2. Register
3. Login
4. Account pages
5. Thank-you pages

SEO titles and meta descriptions must follow:

`content/COPYWRITING_RULES.md`

---

### Task 19: Blog Category Structure

Create blog categories:

1. Growth Systems
2. Brand Positioning
3. AI Leverage
4. Customer Journey
5. Content Systems
6. Business Clarity
7. Personal Brand

Important:

SEO is the architecture behind the blog.

SEO is not the blog topic itself.

Category copy must follow:

`content/COPYWRITING_RULES.md`

---

### Task 20: Internal Linking

Add internal links across pages.

Priority links:

1. Home to Growth Systems
2. Home to Modules
3. Home to Contact
4. Growth Systems to Modules
5. Modules to Contact
6. Blog to Growth Systems
7. Courses to Dashboard
8. Studio to Contact
9. About to Work and Studio
10. Footer to all key pages

Anchor text should feel natural and premium.

Avoid generic link text.

---

## Phase 9: n8n Automation Preparation

### Task 21: Prepare Automation Events

Reference:

`n8n/AUTOMATION_ARCHITECTURE.md`

Track these events:

1. Newsletter subscription
2. Contact form submission
3. Growth Diagnosis submission
4. Strategy call booking
5. Course registration
6. Webinar registration
7. Resource download
8. Dashboard activity
9. Member offer click

---

### Task 22: Define Data Fields

Capture:

1. Name
2. Email
3. Company
4. Website
5. Source page
6. CTA clicked
7. Interest category
8. Growth challenge
9. Inquiry type
10. UTM source
11. UTM campaign
12. Consent
13. Timestamp

---

### Task 23: Connect Forms to n8n Later

MVP can start with email notifications.

Later connect forms to:

1. n8n webhook
2. CRM
3. Google Sheets
4. Email sequence
5. Lead segmentation
6. Dashboard status update

Automation messages and confirmation emails must follow:

`content/COPYWRITING_RULES.md`

---

## Phase 10: Content and Visual QA

### Task 24: Copy Quality Check

Every page must avoid:

1. Robotic wording
2. AI clichés
3. Generic agency language
4. Overhyped AI claims
5. Social media manager positioning
6. Freelancer-style copy
7. Public copy with dashes
8. Pushy sales language
9. Cheap CTA language
10. Artificially polished sentences

Every page must feel:

1. Human
2. Strategic
3. Premium
4. Clear
5. Confident
6. Business-oriented
7. Natural
8. Trustworthy

Use:

`content/COPYWRITING_RULES.md`

---

### Task 25: Design Quality Check

Every page must feel:

1. Spacious
2. Minimal
3. Premium
4. Executive
5. Clean
6. Calm
7. System-oriented

Avoid:

1. Crowded sections
2. Generic stock images
3. Heavy gradients
4. Loud animation
5. Cheap icons
6. Template-heavy layout
7. Agency-style clutter

---

### Task 26: Mobile QA

Check every page on mobile.

Required:

1. Header works
2. Hamburger works
3. CTA visible
4. Text readable
5. Forms usable
6. Cards stack cleanly
7. Footer not too long or messy
8. No horizontal scroll
9. Dashboard usable
10. Booking flow usable

---

### Task 27: Performance QA

Check:

1. Image size
2. Plugin load
3. CSS size
4. JavaScript load
5. Mobile speed
6. Elementor section complexity
7. Cache plugin setup
8. Font loading
9. Lazy loading

Avoid:

1. Heavy sliders
2. Auto-playing videos
3. Too many effects
4. Too many plugins
5. Large uncompressed images
6. Unnecessary animation libraries

---

### Task 28: Accessibility QA

Check:

1. Heading hierarchy
2. Button labels
3. Link clarity
4. Form labels
5. Color contrast
6. Keyboard navigation
7. Reduced motion behavior
8. Focus states
9. Mobile tap targets
10. Error message clarity

Microcopy must follow:

`content/COPYWRITING_RULES.md`

---

## Phase 11: Launch Preparation

### Task 29: Legal Pages

Create:

1. Privacy Policy
2. Terms of Use
3. Cookie Policy if needed

Important because the site collects:

1. Newsletter subscriptions
2. Contact form data
3. User registration data
4. Course and webinar interest
5. Dashboard activity later

Legal copy should be clear, professional, and trustworthy.

---

### Task 30: Final Launch Checklist

Before launch:

1. All key pages published
2. Header and footer active
3. Forms tested
4. Booking tested
5. SEO titles and meta descriptions added
6. Mobile checked
7. Speed checked
8. Links checked
9. Dashboard noindexed
10. Login and register tested
11. Newsletter form tested
12. Analytics added if needed
13. Backup configured
14. Copy checked against `content/COPYWRITING_RULES.md`
15. No public website copy uses dashes
16. No public website copy sounds robotic or AI-generated

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

1. Courses
2. Webinars
3. Dashboard
4. Account system
5. Saved resources
6. Member-only offers
7. n8n CRM workflows
8. Course-to-consulting automation
9. Advanced SEO blog system
10. YouTube and Skool integration

---

## Final Build Rule

Do not build random pages.

Do not add features because they are trendy.

Do not make the site look like an agency template.

Do not publish public website copy before checking:

`content/COPYWRITING_RULES.md`

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
