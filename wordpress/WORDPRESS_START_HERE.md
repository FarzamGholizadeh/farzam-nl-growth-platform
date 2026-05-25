# WordPress Start Here

## Purpose

This document is the practical starting point for building Farzam.nl inside WordPress.

Use this file when entering WordPress for the first time and starting the actual website build.

The goal is to move from repository planning into real WordPress and Elementor execution without losing the strategic direction.

Farzam.nl must be built as a premium Growth System platform.

Not a portfolio.

Not an agency website.

Not an AI tool website.

---

## Start With These Files

Before touching WordPress, read these files in this order:

1. `README.md`
2. `AGENTS.md`
3. `content/COPYWRITING_RULES.md`
4. `tasks/WORDPRESS_ELEMENTOR_BUILD_TASKS.md`
5. `elementor/ELEMENTOR_IMPLEMENTATION_GUIDE.md`
6. `wordpress/WORDPRESS_STACK.md`
7. `elementor/custom-css/FARZAM_GLOBAL_STYLE.md`
8. `elementor/custom-js/FARZAM_PREMIUM_MOTION.md`

Before writing any visible website text, always read:

`content/COPYWRITING_RULES.md`

---

## Core Reminder

Farzam.nl must position Farzam as:

1. Growth Strategist
2. Growth System Designer
3. Business-Oriented Thinker

The website must not position Farzam as:

1. Traditional marketer
2. Freelance marketer
3. Social media manager
4. AI tool operator
5. Generic agency owner

Core message:

Build a Growth System, not just more marketing.

Marketing, content, AI, automation, websites, and campaigns are tools inside the Growth System.

They are not the identity of the brand.

---

## Public Copy Rule

All public website copy must follow:

`content/COPYWRITING_RULES.md`

Main rules:

1. Do not use dashes.
2. Do not use AI-sounding language.
3. All text must feel human, natural, professional, and premium.
4. Avoid robotic sentence structures.
5. Avoid generic AI phrases.
6. Avoid over-polished artificial wording.
7. Write like a strategic human consultant.
8. Keep the tone clear, calm, executive, and trustworthy.

This applies to:

1. Headlines
2. Subheadlines
3. Paragraphs
4. CTAs
5. Button labels
6. Forms
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

Internal documentation and technical notes may use normal Markdown syntax when needed.

---

## Step 1: Check WordPress Basics

Inside WordPress dashboard, check:

1. WordPress is installed correctly
2. Admin login works
3. SSL is active
4. Website loads without error
5. Theme area is accessible
6. Plugin area is accessible
7. Media library works
8. Permalinks are editable

Recommended permalink setting:

`/%postname%/`

Path:

Settings  
→ Permalinks  
→ Post name  
→ Save Changes

---

## Step 2: Set Basic Site Settings

Go to:

Settings  
→ General

Set:

1. Site Title: Farzam Gholizadeh
2. Tagline: Growth Strategist and Growth System Designer
3. Site Language: English
4. Timezone: Amsterdam or Netherlands time
5. Date format: clean and readable
6. Time format: clean and readable

Then save.

---

## Step 3: Install Core Plugins

Install these first:

1. Elementor
2. Elementor Pro
3. Yoast SEO
4. Code Snippets or similar custom code plugin
5. Backup plugin
6. Security plugin
7. Cache or performance plugin

Optional later:

1. Ultimate Member or ProfilePress
2. Tutor LMS or LearnDash
3. FluentBooking or Calendly embed
4. WooCommerce if paid courses are added later
5. Newsletter or CRM integration plugin if needed

Do not install too many plugins at the beginning.

Keep the website lightweight.

---

## Step 4: Choose a Clean Theme

Use a lightweight Elementor-friendly theme.

Recommended options:

1. Hello Elementor
2. Astra
3. GeneratePress
4. Kadence

MVP recommendation:

Hello Elementor

Reason:

It gives Elementor full control and keeps the site clean.

---

## Step 5: Configure Elementor Global Settings

Go to:

Elementor  
→ Site Settings

Use reference:

`elementor/custom-css/FARZAM_GLOBAL_STYLE.md`

Configure:

1. Global colors
2. Global fonts
3. Typography scale
4. Button styles
5. Form styles
6. Container width
7. Layout spacing
8. Responsive settings

Recommended container widths:

1. Standard container: 1180px
2. Wide container: 1320px

Visual direction:

1. Premium
2. Minimal
3. Executive
4. Spacious
5. Calm
6. Light
7. Strategic
8. System-oriented

---

## Step 6: Add Global CSS

Use the CSS direction from:

`elementor/custom-css/FARZAM_GLOBAL_STYLE.md`

Add CSS through one of these:

1. Elementor Site Settings Custom CSS
2. WordPress Customizer Additional CSS
3. Code Snippets
4. Child theme stylesheet later

Use consistent classes:

1. `fgs-section`
2. `fgs-container`
3. `fgs-container-wide`
4. `fgs-card`
5. `fgs-btn-primary`
6. `fgs-btn-secondary`
7. `fgs-form`
8. `fgs-reveal`
9. `fgs-stagger`

Do not create random class names unless necessary.

---

## Step 7: Add Premium Motion

Use reference:

`elementor/custom-js/FARZAM_PREMIUM_MOTION.md`

Add JavaScript through:

1. Elementor Custom Code
2. Code Snippets
3. Child theme later

Motion must be:

1. Calm
2. Subtle
3. Premium
4. Lightweight
5. Accessible
6. Non-distracting

Avoid:

1. Heavy parallax
2. Neon effects
3. Bouncy animations
4. AI particles
5. Scroll hijacking
6. Auto-moving sliders

---

## Step 8: Create WordPress Pages

Create these pages:

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

1. Home: `/`
2. Growth Systems: `/growth-systems`
3. Modules: `/modules`
4. Work: `/work`
5. Blog: `/blog`
6. Courses: `/courses`
7. Studio: `/studio`
8. About: `/about`
9. Contact: `/contact`
10. Dashboard: `/dashboard`
11. Register: `/register`
12. Login: `/login`

---

## Step 9: Set Home and Blog Pages

Go to:

Settings  
→ Reading

Set:

1. Your homepage displays: A static page
2. Homepage: Home
3. Posts page: Blog

Then save.

---

## Step 10: Build Global Header First

Use Elementor Pro Theme Builder.

Reference:

`elementor/components/HEADER_NAVIGATION.md`

Visible header items:

1. Logo
2. Hamburger Menu
3. Register / Sign In
4. Book a Strategy Call

Header rules:

1. Keep it minimal
2. Keep it premium
3. Keep it sticky if appropriate
4. Do not add full navigation links in the top bar
5. Put all main links inside the hamburger menu
6. Make Book a Strategy Call visible
7. Make Register / Sign In visible

Hamburger menu should include:

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

---

## Step 11: Build Global Footer Second

Use Elementor Pro Theme Builder.

Reference:

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

Footer must feel:

1. Clean
2. Structured
3. Premium
4. Calm
5. Useful
6. Easy to scan

---

## Step 12: Build Home Page

Use reference:

`elementor/page-blueprints/HOME.md`

Purpose:

The Home page introduces Farzam’s positioning and explains why Growth Systems matter.

Home page must answer:

1. Who is Farzam helping?
2. What is the problem?
3. What is a Growth System?
4. Why is this different from more marketing activity?
5. What should the visitor do next?

Primary CTA:

Book a Strategy Call

Secondary CTA:

Explore Growth Systems

Before writing copy:

Read `content/COPYWRITING_RULES.md`

---

## Step 13: Build Growth Systems Page

Use reference:

`elementor/page-blueprints/GROWTH_SYSTEMS.md`

Purpose:

This page explains the core methodology.

It must clarify:

1. What a Growth System is
2. Why businesses need one
3. How strategy, positioning, customer journey, content, AI, and automation connect
4. Why marketing and AI are only parts of the system

This is one of the most important pages.

Before writing copy:

Read `content/COPYWRITING_RULES.md`

---

## Step 14: Build Modules Page

Use reference:

`elementor/page-blueprints/MODULES.md`

Purpose:

Show Farzam’s strategic capability areas without making the page feel like a generic service page.

Each module should connect:

1. Business problem
2. Strategic diagnosis
3. System design
4. Practical outcome

Before writing copy:

Read `content/COPYWRITING_RULES.md`

---

## Step 15: Build Contact Page Early

Use reference:

`elementor/page-blueprints/CONTACT.md`

Purpose:

Create the main conversion path.

Contact page should include:

1. Strategy call CTA
2. Growth Diagnosis form
3. General contact form
4. Course or webinar inquiry path
5. Collaboration inquiry path

The page must feel like the start of a serious strategic conversation.

Before writing copy:

Read `content/COPYWRITING_RULES.md`

---

## Step 16: Build Blog Structure

Use reference:

`elementor/page-blueprints/BLOG.md`

Create categories:

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

Before writing blog copy:

Read `content/COPYWRITING_RULES.md`

---

## Step 17: Build Remaining Pages

After Home, Growth Systems, Modules, Contact, and Blog structure, build:

1. Courses
2. Studio
3. About
4. Work
5. Dashboard
6. Register
7. Login

Use references:

1. `elementor/page-blueprints/COURSES.md`
2. `elementor/page-blueprints/STUDIO.md`
3. `elementor/page-blueprints/ABOUT.md`
4. `elementor/page-blueprints/WORK.md`
5. `elementor/page-blueprints/DASHBOARD.md`

Dashboard, Register, and Login should be noindex.

---

## Step 18: Configure Yoast SEO

Use reference:

`seo/SEO_ARCHITECTURE.md`

For each public page, set:

1. SEO title
2. Meta description
3. Clean slug
4. One H1
5. Clear heading hierarchy
6. Internal links
7. Natural keyword focus

Noindex:

1. Dashboard
2. Register
3. Login
4. Account pages
5. Thank-you pages

SEO descriptions must follow:

`content/COPYWRITING_RULES.md`

---

## Step 19: Build Forms

Main forms:

1. Growth Diagnosis Form
2. Contact Form
3. Newsletter Signup Form
4. Strategy Call Booking
5. Course Interest Form later
6. Webinar Registration Form later

Form text must be:

1. Clear
2. Calm
3. Human
4. Professional
5. Not pushy

Before writing form copy:

Read `content/COPYWRITING_RULES.md`

---

## Step 20: Prepare n8n Later

Use reference:

`n8n/AUTOMATION_ARCHITECTURE.md`

For MVP, forms can first send email notifications.

Later connect to n8n:

1. Newsletter subscription
2. Contact form submission
3. Growth Diagnosis submission
4. Strategy call booking
5. Course registration
6. Webinar registration
7. Resource download
8. Dashboard activity
9. Member offer click

Automation messages must not sound robotic.

---

## Step 21: Mobile QA

Check every page on mobile.

Required:

1. Header works
2. Hamburger works
3. CTAs are visible
4. Text is readable
5. Forms are usable
6. Cards stack cleanly
7. Footer is not messy
8. No horizontal scroll
9. Booking flow works
10. Page speed is acceptable

---

## Step 22: Copy QA

Before publishing any page, check:

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

Use:

`content/COPYWRITING_RULES.md`

---

## Step 23: Design QA

Before publishing any page, check:

1. Is the page spacious?
2. Is the hierarchy clear?
3. Does it feel premium?
4. Does it avoid agency-template clutter?
5. Does it avoid generic stock images?
6. Does motion feel calm?
7. Are CTAs clear?
8. Is the typography clean?
9. Is spacing consistent?
10. Does the page support the Growth System positioning?

---

## Step 24: MVP Launch Scope

For MVP, prioritize:

1. Header
2. Footer
3. Home
4. Growth Systems
5. Modules
6. Contact
7. Blog structure
8. Basic newsletter form
9. Growth Diagnosis form
10. Strategy Call CTA

Phase 2:

1. Courses
2. Webinars
3. Dashboard
4. Register and Login
5. Account system
6. Saved resources
7. Member-only offers
8. n8n automation
9. LMS
10. YouTube and Skool integration

---

## Final Start Rule

Do not start by designing random sections.

Do not start by installing too many plugins.

Do not start by writing generic marketing copy.

Start with:

1. WordPress foundation
2. Elementor global settings
3. Header
4. Footer
5. Home
6. Growth Systems
7. Modules
8. Contact

Every decision should support the same system:

Visitor  
→ Understand  
→ Trust  
→ Learn  
→ Register  
→ Diagnose  
→ Book  
→ Convert

Farzam.nl is the digital Growth System behind Farzam’s personal brand and consulting ecosystem.
