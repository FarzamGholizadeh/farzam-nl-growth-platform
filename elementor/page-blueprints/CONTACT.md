# Contact Page Blueprint

## Page

Contact `/contact`

## Page Objective

The Contact page must convert qualified visitors into strategic conversations, Growth Diagnosis submissions, consulting leads, course/webinar inquiries, or collaboration opportunities.

This page should feel calm, premium, and serious. It should not feel like a generic contact form.

The main goal is to help visitors take the right next step based on their situation.

---

## Target User Intent

Visitors on this page may want to:

- Book a Strategy Call
- Complete a Growth Diagnosis
- Ask about collaboration
- Ask about courses or webinars
- Discuss a project
- Understand how working with Farzam starts
- Contact Farzam directly

---

## SEO Intent

Primary keyword theme:
Book growth strategy call

Supporting topics:
- Growth diagnosis
- Growth consulting
- Strategy call
- Business growth consultation
- Growth system audit
- Brand positioning consultation
- AI workflow consultation

Suggested H1:
Start a Strategic Conversation

Suggested meta title:
Contact Farzam | Book a Growth Strategy Call

Suggested meta description:
Book a strategy call with Farzam to diagnose where growth is broken and explore how a structured Growth System can help your business move forward.

---

## Hero Section

### Section Goal

Make the page feel like the start of a serious strategic conversation.

### H1

Start a Strategic Conversation

### Subheadline

If your growth feels scattered, your positioning is unclear, your content lacks structure, or your team is using tools without a connected system, the first step is diagnosis.

### Primary CTA

Book a Strategy Call

### Secondary CTA

Complete Growth Diagnosis

### Design Notes

- Premium light background
- Calm tone
- Clear CTA buttons
- Avoid aggressive sales language
- Motion: soft fade-in only

---

## Section 2: Choose Your Next Step

### Section Goal

Help visitors select the right action.

### Suggested H2

Choose the path that fits your situation.

### Path Cards

1. Book a Strategy Call
   - For businesses ready to discuss a specific growth challenge

2. Complete Growth Diagnosis
   - For visitors who are not sure where growth is breaking

3. Ask About Courses or Webinars
   - For learning-focused visitors

4. Collaboration Inquiry
   - For partnerships, projects, or strategic work

### CTA

Select Your Path

### Design Notes

- Use clean cards
- Each card should have one clear CTA
- Keep the wording serious and premium

---

## Section 3: Growth Diagnosis Form

### Section Goal

Capture qualified information before a conversation.

### Suggested H2

Diagnose where your growth system may be breaking.

### Copy Direction

Position the form as a strategic first step. The visitor should feel that this is not a random contact form, but a structured way to clarify their growth challenge.

### Recommended Fields

- Name
- Email
- Company / project
- Website
- Business type
- Current growth challenge
- Where does growth feel broken?
- Main priority
- Current marketing maturity
- AI / automation usage
- Team size
- Budget range
- Desired outcome
- Preferred collaboration type
- Message

### Field Type Suggestions

- Business type: dropdown
- Current growth challenge: multi-select
- Where growth feels broken: multi-select
- Main priority: dropdown
- Marketing maturity: dropdown
- AI / automation usage: dropdown
- Budget range: optional dropdown
- Preferred collaboration type: dropdown

### Primary CTA

Submit Growth Diagnosis

### n8n Trigger

growth_diagnosis_intake

---

## Section 4: Strategy Call Booking

### Section Goal

Allow high-intent users to book directly.

### Suggested H2

Ready to talk through the system?

### Copy Direction

Explain what the strategy call is for and what it is not.

The call is for:
- Understanding the current growth challenge
- Identifying where the system may be blocked
- Exploring whether Farzam can help
- Defining the next practical step

The call is not:
- A generic sales pitch
- A free execution plan
- A tactical marketing checklist

### Booking Tool Direction

Use:
- Calendly embed
- FluentBooking
- Amelia

MVP Recommendation:
Calendly or FluentBooking.

### Primary CTA

Book a Strategy Call

### n8n Trigger

strategy_call_booking

---

## Section 5: General Contact Form

### Section Goal

Provide a simpler path for general inquiries.

### Suggested H2

For general inquiries

### Recommended Fields

- Name
- Email
- Company / project
- Website
- Inquiry type
- Message
- Consent checkbox

### Inquiry Type Options

- Strategy call
- Growth Diagnosis
- Course or webinar
- Collaboration
- Speaking / workshop
- Other

### Primary CTA

Send Message

### n8n Trigger

contact_form_submission

---

## Section 6: What Happens After You Submit

### Section Goal

Reduce uncertainty and build trust.

### Suggested H2

What happens next?

### Process Steps

1. You submit your request
2. Farzam reviews the context
3. You receive a confirmation email
4. If relevant, you receive a booking link or next-step recommendation
5. The conversation focuses on diagnosis, clarity, and practical direction

### Design Notes

- Use simple step cards
- Keep the tone calm and clear
- Avoid overpromising

---

## Section 7: Who This Is Best For

### Section Goal

Qualify the right audience.

### Suggested H2

This is best for businesses and experts that need structure.

### Audience Cards

1. SMEs with unclear growth direction
2. Startups needing positioning and GTM clarity
3. Experts building a personal brand system
4. Teams with scattered marketing execution
5. Businesses exploring AI and automation with purpose
6. Founders needing a clearer customer journey

---

## Section 8: Final Trust Block

### Section Goal

Reinforce credibility before the final CTA.

### Suggested H2

The goal is clarity before execution.

### Copy Direction

Explain that Farzam’s approach starts by understanding the business and diagnosing the system. The goal is to avoid random marketing activity and build a clearer path forward.

### CTA

Start with Diagnosis

---

## Elementor Layout Notes

Use Elementor Pro with:

- Hero section
- Path selection cards
- Growth Diagnosis form
- Strategy call booking block
- General contact form
- What happens next section
- Audience qualification cards
- Final CTA block

Layout direction:
- Keep page calm and spacious
- Use strong form hierarchy
- Avoid long intimidating form design
- If the Growth Diagnosis form is long, use multi-step form design
- Keep mobile form experience clean

---

## Motion Notes

Allowed:
- Calm hero reveal
- Soft card hover
- Smooth form step transition
- Gentle booking block reveal

Avoid:
- Flashy form animations
- Distracting motion around forms
- Heavy parallax

---

## n8n Automation Entry Points

This page should support:

1. Growth Diagnosis form
2. Contact form
3. Strategy call booking
4. Course/webinar inquiry
5. Collaboration inquiry

Data to capture:
- Source page: Contact
- Form type
- Inquiry type
- Growth challenge
- Interest category
- UTM source
- UTM campaign
- Consent
- Booking status if applicable

---

## Internal Linking Summary

This page should link to:

- `/growth-systems`
- `/modules`
- `/courses`
- `/blog`
- `/work`

---

## Success Criteria

The Contact page is successful when:

- Visitors know exactly how to start
- High-intent visitors can book a Strategy Call
- Unclear visitors can complete Growth Diagnosis
- Learning-focused visitors can ask about courses or webinars
- Form data is useful for n8n segmentation
- The page feels premium, calm, and trustworthy
