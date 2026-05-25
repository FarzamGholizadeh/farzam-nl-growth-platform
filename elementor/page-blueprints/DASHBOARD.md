# User Dashboard Blueprint

## Page

User Dashboard `/dashboard`

## Page Objective

The Dashboard must give registered users a simple, premium, and structured account experience.

This section should not feel like a generic WordPress account page. It should feel like a calm learning and growth hub where users can access courses, webinars, saved resources, newsletter preferences, Growth Diagnosis status, and member-only strategy offers.

The Dashboard should support Farzam.nl’s larger platform logic:

Visitor → Register → Learn → Engage → Diagnose → Book Strategy Call → Become Client

---

## Target User Intent

Registered users may want to:

- Access their courses
- Join webinars
- Save resources
- Manage newsletter preferences
- See their Growth Diagnosis status
- Access member-only offers
- Book a strategy call
- Continue learning from Farzam’s frameworks

---

## SEO Intent

The dashboard should not be indexed.

Recommended SEO setting:
- Noindex
- Nofollow if needed
- Private / account-only access

Reason:
The dashboard is user-specific and should not appear in search results.

---

## User Access

The dashboard should be accessible only after user registration or sign in.

Possible user states:

1. Logged out
   - Show Register / Sign In prompt

2. Logged in, new user
   - Show onboarding and recommended next steps

3. Logged in, active learner
   - Show courses, webinars, resources, and offers

4. Logged in, consulting lead
   - Show Growth Diagnosis status and strategy call CTA

---

## Dashboard Hero / Welcome Area

### Section Goal

Welcome the user and orient them quickly.

### Suggested H1

Welcome back.

### Personalized Direction

If possible, use:

Welcome back, [First Name].

### Subheadline

Continue your learning path, access saved resources, and take the next step toward building a clearer Growth System.

### Primary CTA

Continue Learning

### Secondary CTA

Book a Strategy Call

### Design Notes

- Clean dashboard header
- Minimal UI
- Use user name if available
- No clutter
- Calm premium interface

---

## Section 2: Dashboard Navigation

### Section Goal

Give users simple access to account areas.

### Dashboard Navigation Items

- Overview
- My Courses
- My Webinars
- Saved Resources
- Growth Diagnosis
- Newsletter Preferences
- Strategy Offer
- Account Settings

### Design Notes

Desktop:
- Sidebar or horizontal tabs

Mobile:
- Dropdown or stacked navigation

Keep navigation minimal and clear.

---

## Section 3: My Courses

### Section Goal

Show courses the user has registered for or can access.

### Suggested H2

My Courses

### Course Card Fields

Each course card should include:

- Course title
- Progress status
- Course type
- Last accessed
- CTA: Continue Course
- CTA: View Details

### Empty State

If user has no courses:

Suggested copy:
You have not joined any courses yet. Explore free resources, mini courses, and webinars to start building your Growth System.

CTA:
Explore Courses

Internal link:
`/courses`

---

## Section 4: My Webinars

### Section Goal

Show registered webinars and upcoming learning sessions.

### Suggested H2

My Webinars

### Webinar Card Fields

- Webinar title
- Date
- Time
- Status
- Join link if available
- Replay link if available
- CTA: View Webinar

### Empty State

Suggested copy:
No webinars registered yet. Join a live session to go deeper into Growth Systems, positioning, AI leverage, and content systems.

CTA:
Join the Next Webinar

Internal link:
`/courses`

---

## Section 5: Saved Resources

### Section Goal

Let users access downloaded or saved materials.

### Suggested H2

Saved Resources

### Resource Types

- Growth Audit Checklist
- Positioning Clarity Worksheet
- Customer Journey Map
- Content System Planner
- AI Workflow Starter Map
- Blog Repurposing Template
- Strategy Call Preparation Sheet

### Resource Card Fields

- Resource title
- Category
- Short description
- Download / View CTA

### Empty State

Suggested copy:
You have not saved any resources yet. Start with a free Growth System resource.

CTA:
Explore Resources

Internal link:
`/courses`

---

## Section 6: Growth Diagnosis Status

### Section Goal

Connect dashboard activity to consulting conversion.

### Suggested H2

Growth Diagnosis

### Possible States

1. Not started
   - CTA: Start Growth Diagnosis

2. Submitted
   - Message: Your Growth Diagnosis has been received.

3. Reviewed
   - Message: Your diagnosis has been reviewed. Book a Strategy Call to discuss the next step.

4. Strategy call booked
   - Show date and next step

### Fields to Display

- Submission date
- Diagnosis category if available
- Status
- Recommended next step
- CTA

### Primary CTA

Start Growth Diagnosis

### Secondary CTA

Book a Strategy Call

---

## Section 7: Newsletter Preferences

### Section Goal

Allow users to manage what kind of strategic content they receive.

### Suggested H2

Newsletter Preferences

### Interest Categories

- Growth Systems
- Brand Positioning
- AI Leverage
- Customer Journey
- Content Systems
- Business Clarity
- Personal Brand
- Courses and Webinars

### Settings

- Subscribe / unsubscribe
- Select topics
- Email frequency if available

### n8n Trigger

newsletter_preferences_updated

---

## Section 8: Member-only Strategy Offer

### Section Goal

Create a premium conversion path for registered users.

### Suggested H2

Member-only Strategy Offer

### Copy Direction

Avoid cheap discount language.

Use premium positioning:

As a registered member, you may access selected strategy offers, early webinar invitations, and priority access to Growth Diagnosis sessions.

### Offer Types

- Priority Growth Diagnosis
- Reduced-rate Strategy Session
- Early access to workshops
- Course-to-consulting session
- Private review session

### Primary CTA

Book Your Strategy Session

### Secondary CTA

Complete Growth Diagnosis

---

## Section 9: Recommended Next Steps

### Section Goal

Guide users based on their activity.

### Suggested H2

Recommended next steps

### Logic Examples

If user has no course:
- Explore Courses

If user has course but no diagnosis:
- Complete Growth Diagnosis

If user completed diagnosis but no call:
- Book Strategy Call

If user joined newsletter only:
- Start with Growth System Foundations

If user attended webinar:
- Apply for Strategy Session

### Design Notes

Use simple recommendation cards.

---

## Section 10: Account Settings

### Section Goal

Give users basic account control.

### Recommended Fields

- Name
- Email
- Password update
- Newsletter consent
- Account preferences
- Delete account request if needed

### Privacy Note

Make account data handling clear and professional.

---

## Elementor Layout Notes

Use Elementor Pro with:

- Dashboard wrapper
- User welcome block
- Dashboard navigation
- Course cards
- Webinar cards
- Resource cards
- Diagnosis status card
- Newsletter preferences form
- Strategy offer card
- Account settings block

Important:
The dashboard may require membership/account plugin templates rather than pure Elementor pages.

Recommended plugins:
- Ultimate Member
- ProfilePress
- Paid Memberships Pro
- Tutor LMS or LearnDash later

---

## Motion Notes

Allowed:
- Calm card reveal
- Subtle hover states
- Smooth tab switching
- Gentle status updates

Avoid:
- Gamified animations
- Flashy dashboard effects
- Heavy motion
- Noisy UI

---

## n8n Automation Entry Points

The Dashboard should support:

1. User registration event
2. Course click tracking
3. Webinar click tracking
4. Resource download tracking
5. Growth Diagnosis status update
6. Newsletter preference update
7. Member strategy offer click
8. Strategy call booking

Data to capture:
- User ID
- Email
- Action type
- Course ID if applicable
- Webinar ID if applicable
- Resource ID if applicable
- Diagnosis status
- CTA clicked
- Timestamp

---

## Internal Linking Summary

Dashboard should link to:

- `/courses`
- `/blog`
- `/growth-systems`
- `/contact`

---

## Success Criteria

The Dashboard is successful when:

- Registered users understand what to do next
- Courses, webinars, and resources are easy to access
- Newsletter preferences are clear
- Growth Diagnosis creates a path toward consulting
- Member-only offers feel premium, not cheap
- The dashboard supports n8n segmentation and lead nurturing
- The experience feels simple, calm, and professional
