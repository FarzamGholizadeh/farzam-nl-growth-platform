# Farzam.nl n8n Automation Architecture

## Purpose

This document defines the automation architecture for Farzam.nl.

The website should not only describe Growth Systems. It should operate like one.

n8n will connect website forms, registrations, courses, webinars, newsletter subscriptions, CRM, email marketing, and content repurposing into one structured growth engine.

---

## Core Automation Logic

Primary system flow:

Visitor → Lead Capture → Segmentation → Email Nurture → CRM Pipeline → Strategy Call → Proposal → Client

Secondary system flow:

Content → Blog → Newsletter → Social Repurposing → Audience Growth → Lead Capture

Education system flow:

YouTube / Skool / Blog → Courses → Register → Webinar / Course → Member Offer → Consulting Lead

---

## Automation Entry Points

The website should include these automation entry points:

1. Contact form
2. Growth Diagnosis form
3. Newsletter signup
4. User registration
5. Course registration
6. Webinar registration
7. Lead magnet download
8. Strategy call booking
9. Blog subscription CTA
10. Member-only strategy offer
11. Course completion event
12. Webinar attendance event

---

## 1. Contact Form Automation

### Trigger

Elementor form, Fluent Forms, Gravity Forms, or WP Webhooks sends data to n8n webhook.

### Fields

- Name
- Email
- Company
- Website
- Message
- Collaboration type
- Budget range
- Source page
- UTM source
- UTM campaign

### n8n Actions

1. Receive webhook
2. Validate required fields
3. Create or update contact
4. Tag lead source
5. Add to CRM pipeline
6. Send confirmation email
7. Notify Farzam
8. Add follow-up reminder if no response

### Suggested Tags

- contact_form
- consulting_interest
- source_contact_page

---

## 2. Growth Diagnosis Form Automation

### Trigger

Growth Diagnosis form submitted.

### Purpose

Diagnose where the user’s growth system is broken and segment them for follow-up.

### Fields

- Name
- Email
- Company
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
- Source page
- UTM source

### Diagnosis Categories

Possible segments:
- positioning_problem
- customer_journey_problem
- content_system_problem
- conversion_problem
- ai_automation_opportunity
- business_clarity_problem
- execution_system_problem

### n8n Actions

1. Receive form payload
2. Normalize fields
3. Score lead based on answers
4. Assign diagnosis category
5. Create CRM opportunity
6. Notify Farzam with summary
7. Send confirmation email to lead
8. Send booking link
9. If no booking after 48 hours, send reminder
10. If no booking after 7 days, add to nurture sequence

### Lead Score Example

High-intent signals:
- Budget selected
- Company website provided
- Strategy call requested
- Urgent growth problem selected
- Team or business context provided

Low-intent signals:
- No company data
- No budget
- General curiosity only

---

## 3. Newsletter Signup Automation

### Trigger

Newsletter form submitted.

### Newsletter Name

Growth Systems Letter

### Fields

- Name
- Email
- Interest category
- Source page
- UTM source
- Consent checkbox

### Interest Categories

- Growth Systems
- Brand Positioning
- AI Leverage
- Customer Journey
- Content Systems
- Business Clarity
- Personal Brand
- Courses and Webinars

### n8n Actions

1. Add subscriber to email platform
2. Add interest tags
3. Add source tag
4. Send welcome email
5. Start interest-based nurture sequence
6. Track engagement
7. Increase lead score based on clicks

### Suggested Tags

- newsletter_subscriber
- interest_growth_systems
- interest_positioning
- interest_ai_leverage
- interest_courses

---

## 4. User Registration Automation

### Trigger

User creates account.

### Fields

- Name
- Email
- User role
- Registration source
- Selected interests
- Course interest
- Newsletter consent

### n8n Actions

1. Create or update user record
2. Add registered_user tag
3. Send account welcome email
4. Add to onboarding sequence
5. If course selected, trigger course registration flow
6. If webinar selected, trigger webinar registration flow
7. If newsletter consent true, add to Growth Systems Letter

### Suggested Tags

- registered_user
- dashboard_user
- learner
- member

---

## 5. Course Registration Automation

### Trigger

User enrolls in free or paid course.

### Course Types

- Free course
- Paid course
- Mini course
- Workshop
- Webinar-based course

### Fields

- User ID
- Name
- Email
- Course ID
- Course name
- Course type
- Payment status
- Enrollment date
- Source page

### n8n Actions

1. Confirm user registration
2. Add course tag
3. Send course access email
4. Add to course onboarding sequence
5. Track progress if LMS supports events
6. Trigger consulting offer after engagement milestone

### Example Tags

- course_enrolled
- course_free
- course_paid
- course_growth_systems
- course_ai_workflows

---

## 6. Webinar Registration Automation

### Trigger

User registers for webinar.

### Fields

- Name
- Email
- Webinar name
- Webinar date
- Source
- Registration status

### n8n Actions

1. Add webinar_registered tag
2. Send confirmation email
3. Send 24-hour reminder
4. Send 1-hour reminder
5. Send 10-minute reminder if useful
6. After event, segment user:
   - attended
   - no_show
7. Send replay email
8. Send member-only strategy offer
9. Add to CRM if high intent

### Tags

- webinar_registered
- webinar_attended
- webinar_no_show
- webinar_replay_sent

---

## 7. Lead Magnet Automation

### Trigger

User downloads a resource.

### Possible Resources

- Growth Audit Checklist
- Positioning Clarity Worksheet
- Content System Planner
- Customer Journey Map
- AI Workflow Starter Map
- Blog Repurposing Template

### Fields

- Name
- Email
- Resource name
- Topic category
- Source page
- Consent

### n8n Actions

1. Send resource by email
2. Add resource_download tag
3. Add topic segment
4. Start resource-specific nurture sequence
5. Suggest related blog or course
6. Later invite to Growth Diagnosis

---

## 8. Strategy Call Booking Automation

### Trigger

Booking confirmed through Calendly, Amelia, FluentBooking, or similar.

### Fields

- Name
- Email
- Meeting date
- Meeting time
- Time zone
- Booking source
- Form answers if available

### n8n Actions

1. Create CRM deal
2. Add strategy_call_booked tag
3. Send pre-call email
4. Send calendar confirmation if not handled by booking tool
5. Notify Farzam
6. Create pre-call summary
7. After call, trigger follow-up sequence

### Follow-Up Stages

- Call booked
- Call completed
- Proposal needed
- Proposal sent
- Won
- Lost
- Nurture later

---

## 9. Blog to Social Repurposing Automation

### Trigger

New blog post published.

### Fields

- Blog title
- Blog URL
- Category
- Excerpt
- Main points
- Author
- Publish date

### n8n Actions

1. Capture new post
2. Generate newsletter draft
3. Generate LinkedIn post ideas
4. Generate X post thread ideas
5. Generate Instagram carousel outline
6. Generate TikTok / Reels talking points
7. Add to content calendar
8. Optionally create draft tasks in Notion, Google Sheets, or project board

### Important

All AI-generated repurposing must be reviewed manually before publishing.

Farzam’s tone must remain:
- Human
- Strategic
- Premium
- Clear
- Non-robotic

---

## 10. CRM Pipeline Architecture

### Suggested CRM Stages

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

### Lead Score Signals

Positive scoring:
- Completed Growth Diagnosis
- Booked strategy call
- Attended webinar
- Registered for course
- Downloaded multiple resources
- Clicked consulting offer
- Provided budget
- Provided company website

Negative or low-priority signals:
- No engagement after signup
- Fake or incomplete email
- No relevant business context
- Unsubscribed

---

## 11. Email Sequence Architecture

### Welcome Sequence

Audience:
Newsletter subscribers and registered users.

Emails:
1. Welcome to Growth Systems Letter
2. What a Growth System actually is
3. Why more marketing does not fix broken growth
4. Where growth usually breaks
5. Invitation to Growth Diagnosis

### Course Onboarding Sequence

Emails:
1. Welcome and access details
2. How to use the course
3. Key framework introduction
4. Related resources
5. Member-only Strategy Offer

### Webinar Sequence

Emails:
1. Confirmation
2. 24-hour reminder
3. 1-hour reminder
4. Replay and resources
5. Strategy offer
6. Follow-up if no booking

### Growth Diagnosis Follow-Up

Emails:
1. Confirmation and next step
2. Book your Strategy Call
3. Reminder after 48 hours
4. Strategic content based on diagnosis segment
5. Long-term nurture if no booking

---

## 12. Recommended n8n Workflow Structure

Create separate workflows for clarity:

1. `lead-capture-contact-form`
2. `growth-diagnosis-intake`
3. `newsletter-subscription`
4. `user-registration-onboarding`
5. `course-registration-flow`
6. `webinar-registration-flow`
7. `strategy-call-booking-flow`
8. `blog-to-content-repurposing`
9. `lead-scoring-and-crm-update`
10. `email-nurture-router`

---

## 13. Webhook Payload Standards

Every website form should send:

```json
{
  "event_type": "form_submission",
  "form_name": "",
  "name": "",
  "email": "",
  "company": "",
  "website": "",
  "message": "",
  "source_page": "",
  "utm_source": "",
  "utm_medium": "",
  "utm_campaign": "",
  "interest_category": "",
  "consent": true,
  "submitted_at": ""
}
```

Growth Diagnosis should send additional fields:

```json
{
  "growth_challenge": "",
  "growth_break_point": "",
  "business_type": "",
  "team_size": "",
  "budget_range": "",
  "marketing_maturity": "",
  "ai_automation_usage": "",
  "desired_outcome": "",
  "preferred_collaboration_type": ""
}
```
