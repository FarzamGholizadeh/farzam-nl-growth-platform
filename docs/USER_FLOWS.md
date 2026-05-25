# Farzam.nl User Flows

## Purpose

This document defines the main user journeys for Farzam.nl.

The website is not a simple personal website. It is a premium Growth Platform designed to move users from awareness to trust, registration, education, nurturing, and consulting conversion.

Core flow:

Visitor → Understand Growth System → Register / Subscribe → Engage with content or courses → Enter n8n nurture flow → Book Strategy Call → Become client

---

## 1. Visitor from LinkedIn, X, Instagram, or TikTok

### Entry Point

Likely entry pages:
- Home
- Blog article
- Courses page
- Specific campaign landing page
- Contact page

### User Intent

The visitor wants to understand:
- Who Farzam is
- What he does
- Whether he is credible
- Whether his thinking is useful
- How to go deeper

### Ideal Journey

1. Arrives from social content
2. Lands on Home or Blog
3. Reads core positioning:
   - Build a Growth System, not just more marketing
4. Clicks:
   - Growth Systems
   - Blog
   - Courses
   - Book a Strategy Call
5. Registers or subscribes
6. Enters segmented email nurture
7. Receives relevant strategic content
8. Books a strategy call

### Primary CTA

Book a Strategy Call

### Secondary CTA

Join the Growth Systems Letter

### n8n Trigger

Source tag:
- social_linkedin
- social_x
- social_instagram
- social_tiktok

Automation:
- Add lead source
- Segment by content interest
- Send welcome email
- Offer relevant blog/course path

---

## 2. Visitor from Google Search

### Entry Point

Likely entry pages:
- Blog article
- Growth Systems page
- Modules page
- Case study page

### User Intent

The visitor is searching for a specific growth, strategy, positioning, AI leverage, or marketing system problem.

### Ideal Journey

1. Lands on SEO-structured content
2. Reads answer or framework
3. Sees internal link to Growth Systems or Modules
4. Downloads a lead magnet or joins newsletter
5. Receives email sequence based on topic
6. Books a Growth Diagnosis or Strategy Call

### Primary CTA

Diagnose Your Growth System

### Secondary CTA

Download a relevant resource

### n8n Trigger

Source tag:
- organic_google

Automation:
- Capture landing page URL
- Capture search intent category if possible
- Assign topic segment
- Send content-specific nurture sequence

---

## 3. Visitor from YouTube or Skool

### Entry Point

Likely entry pages:
- Courses
- Webinar landing page
- Free resource landing page
- Register page

### User Intent

The visitor wants education, practical frameworks, or deeper access after watching a video or joining a community.

### Ideal Journey

1. Arrives from YouTube or Skool
2. Lands on Courses
3. Chooses:
   - Free course
   - Webinar
   - Workshop
   - Lead magnet
4. Creates account
5. Enters user dashboard
6. Accesses course or webinar
7. Receives follow-up emails
8. Gets member-only Strategy Offer
9. Books call if qualified

### Primary CTA

Create Your Account

### Secondary CTA

Join the Next Webinar

### n8n Trigger

Source tag:
- youtube
- skool

Automation:
- Create learner segment
- Send onboarding email
- Track course/webinar interest
- Offer strategy session after engagement

---

## 4. Blog Reader to Newsletter Subscriber

### Entry Point

- Blog article
- Blog category page

### User Intent

The visitor wants ideas, frameworks, and strategic clarity.

### Ideal Journey

1. Reads blog article
2. Finds relevant internal links
3. Sees newsletter CTA
4. Joins Growth Systems Letter
5. Selects interest categories:
   - Growth Systems
   - Brand Positioning
   - AI Leverage
   - Customer Journey
   - Content Systems
   - Business Clarity
   - Personal Brand
6. Receives welcome email
7. Receives curated content sequence
8. Later receives course, webinar, or strategy call invitation

### Primary CTA

Join the Growth Systems Letter

### Secondary CTA

Explore Growth Systems

### n8n Trigger

Source tag:
- blog_subscriber

Automation:
- Add newsletter subscriber
- Add content category tag
- Send welcome sequence
- Add to monthly newsletter
- Score engagement based on clicks

---

## 5. Course Visitor to Registered User

### Entry Point

- Courses page
- Course detail page
- Webinar page
- Social media course CTA
- YouTube description link
- Skool link

### User Intent

The visitor wants structured learning.

### Ideal Journey

1. Opens Courses page
2. Reviews free and paid courses
3. Clicks course or webinar
4. Registers account
5. Completes profile basics
6. Receives course access
7. Enters onboarding email sequence
8. Sees member-only consulting offer

### Primary CTA

Start Learning

### Secondary CTA

Create Free Account

### n8n Trigger

Source tag:
- course_interest
- registered_user

Automation:
- Create user profile record
- Add course interest
- Send onboarding sequence
- Trigger member offer after engagement milestone

---

## 6. Registered User to Webinar Participant

### Entry Point

- User dashboard
- Courses page
- Email campaign
- Blog CTA
- YouTube / Skool CTA

### User Intent

The user wants live education, interaction, or a deeper strategic session.

### Ideal Journey

1. Registered user sees webinar invitation
2. Clicks Join Webinar
3. Registers for event
4. Receives confirmation email
5. Receives reminders:
   - 24 hours before
   - 1 hour before
   - 10 minutes before
6. Attends webinar
7. Receives replay / resource
8. Receives member-only strategy offer
9. Books strategy call

### Primary CTA

Reserve Your Seat

### Secondary CTA

Get the Replay

### n8n Trigger

Source tag:
- webinar_registered
- webinar_attended
- webinar_no_show

Automation:
- Confirmation email
- Reminder emails
- Attendance tagging
- Replay email
- Follow-up offer sequence

---

## 7. Registered User to Consulting Lead

### Entry Point

- Dashboard
- Courses
- Webinar follow-up
- Newsletter
- Blog CTA
- Member-only strategy offer

### User Intent

The user is warmer and may need strategic help.

### Ideal Journey

1. User consumes content or course
2. Sees member-only Strategy Offer
3. Completes Growth Diagnosis form
4. Gets segmented based on growth problem
5. Books Strategy Call
6. Receives pre-call email
7. Enters CRM pipeline
8. Receives follow-up after call

### Primary CTA

Book Your Strategy Call

### Secondary CTA

Complete Growth Diagnosis

### n8n Trigger

Source tag:
- consulting_interest
- growth_diagnosis_completed

Automation:
- Lead scoring
- Add to CRM pipeline
- Notify Farzam
- Send pre-call questionnaire
- Send follow-up sequence

---

## 8. Growth Diagnosis Form to Strategy Call

### Entry Point

- Home CTA
- Growth Systems page
- Modules page
- Contact page
- Dashboard member offer

### Form Fields

Recommended fields:
- Name
- Email
- Company / project
- Website
- Business type
- Current growth challenge
- Where growth feels broken
- Main priority
- Current marketing maturity
- AI / automation usage
- Team size
- Budget range
- Desired outcome
- Preferred collaboration type

### Segmentation Categories

Possible diagnosis results:
- Positioning problem
- Customer journey problem
- Content system problem
- Conversion problem
- AI / automation opportunity
- Business clarity problem
- Execution system problem

### Ideal Journey

1. User completes Growth Diagnosis form
2. n8n receives form data
3. Lead is segmented
4. Lead score is calculated
5. Farzam receives notification
6. User receives confirmation email
7. User is invited to book a Strategy Call
8. CRM pipeline is updated

### Primary CTA

Book a Strategy Call

### n8n Trigger

Source tag:
- growth_diagnosis

Automation:
- Webhook receives form payload
- Lead score calculation
- Segment assignment
- CRM stage creation
- Email confirmation
- Calendar booking invitation
- Follow-up reminder if no booking

---

## 9. Newsletter Subscriber to Course Buyer

### Entry Point

- Blog CTA
- Free resource
- Website footer
- Pop-up / inline subscription block
- Social campaign

### Ideal Journey

1. User joins newsletter
2. Receives welcome sequence
3. Clicks course-related content
4. Gets course recommendation
5. Opens course page
6. Registers account
7. Buys course or joins webinar
8. Enters course-specific nurture
9. Gets consulting offer later

### Primary CTA

Explore Courses

### n8n Trigger

Source tag:
- newsletter_subscriber
- course_click
- course_purchase

Automation:
- Track email engagement
- Trigger course recommendation
- Add buyer tag
- Send onboarding and upsell sequence

---

## 10. Course or Webinar Participant to Client

### Entry Point

- Course completion
- Webinar attendance
- Replay email
- Dashboard offer

### Ideal Journey

1. User completes a course or attends webinar
2. User receives a strategic follow-up
3. User is invited to complete Growth Diagnosis
4. User receives member-only Strategy Offer
5. User books call
6. Farzam reviews diagnosis before call
7. User becomes proposal opportunity

### Primary CTA

Apply for a Growth System Session

### n8n Trigger

Source tag:
- course_completed
- webinar_attended
- consulting_offer_sent

Automation:
- Trigger consulting offer
- Create CRM opportunity
- Notify Farzam
- Send booking link
- Send reminder if no booking

---

## Key Principle

Every journey should support this logic:

Awareness → Understanding → Trust → Registration → Education → Nurture → Diagnosis → Strategy Call → Client

The website must behave like a Growth System, not just describe one.
