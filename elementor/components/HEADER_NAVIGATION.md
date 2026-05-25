# Header and Navigation Component Blueprint

## Component

Global Header and Navigation

## Purpose

The header must keep Farzam.nl minimal, premium, and focused.

The website has many pages, but the visible navigation should stay simple. Instead of showing all menu items in the top bar, the site should use a hamburger menu.

Visible header items:

1. Logo
2. Hamburger Menu
3. Register / Sign In
4. Book a Strategy Call

---

## Header Goals

The header should:

- Keep the website visually clean
- Support premium consultancy positioning
- Avoid a crowded menu
- Make the main conversion action visible
- Provide easy access to account registration
- Keep navigation simple across desktop and mobile

---

## Desktop Header Structure

### Left Side

Logo

Use the provided Farzam / FGS logo.

Logo behavior:
- Click links to Home `/`
- Keep enough whitespace around logo
- Do not resize too small
- Do not redesign or overdecorate

### Right Side

Visible items:

1. Hamburger Menu
2. Register / Sign In
3. Book a Strategy Call

Recommended order:

Hamburger Menu | Register / Sign In | Book a Strategy Call

---

## Mobile Header Structure

Visible items:

1. Logo
2. Hamburger icon
3. Register / Sign In icon or compact text
4. Book CTA as compact button if space allows

If mobile space is limited:
- Keep Logo
- Keep Hamburger
- Keep Book CTA
- Move Register / Sign In inside hamburger menu or use icon

---

## Hamburger Menu Items

The hamburger menu should include:

- Home `/`
- Growth Systems `/growth-systems`
- Modules `/modules`
- Work `/work`
- Blog `/blog`
- Courses `/courses`
- Studio `/studio`
- About `/about`
- Contact `/contact`

Optional account links:
- Register `/register`
- Sign In `/login`
- Dashboard `/dashboard`

---

## Hamburger Menu Design

The hamburger menu should feel premium and editorial.

Recommended style:

- Full-screen overlay or large side panel
- Light background
- Navy typography
- Clear spacing
- Large readable menu links
- Subtle divider lines
- Smooth open / close motion
- Include short positioning line

Suggested positioning line:

Build a Growth System, not just more marketing.

---

## Header CTA

### Main CTA

Book a Strategy Call

URL:
`/contact`

### Secondary Account CTA

Register / Sign In

URLs:
- `/register`
- `/login`
- `/dashboard` if logged in

---

## Header States

### Logged Out User

Show:

- Register / Sign In

### Logged In User

Replace Register / Sign In with:

- Dashboard

Optional:
- Show user icon or first name if plugin supports it

---

## Sticky Header Behavior

Recommended:

- Header can be sticky
- Keep it slim
- Add slight background blur or solid white on scroll
- Add subtle shadow or border only after scroll
- Do not make it visually heavy

---

## Motion Notes

Allowed:

- Smooth hamburger open / close
- Soft fade-in for menu links
- Subtle button hover
- Small header transition on scroll

Avoid:

- Loud menu animation
- Bouncy hamburger effects
- Heavy parallax
- Flashy transitions

---

## Elementor Implementation Notes

Use Elementor Pro Theme Builder for:

- Global Header
- Global Header conditions across entire site
- Hamburger overlay or popup menu
- Responsive header versions

Possible implementation options:

1. Elementor Popup for hamburger menu
2. Custom HTML / CSS / JS for a lightweight menu
3. Elementor Nav Menu inside full-screen overlay

Recommended MVP:

Use Elementor Pro Popup or Theme Builder first.  
Add custom CSS for premium styling if needed.

---

## Accessibility Notes

Header should support:

- Keyboard navigation
- Clear focus states
- Accessible menu labels
- Close button inside hamburger menu
- Proper aria labels if custom code is used
- Good contrast
- Mobile tap targets large enough

---

## n8n Tracking

Track these interactions later if needed:

- Hamburger menu opened
- Register clicked
- Sign In clicked
- Dashboard clicked
- Book a Strategy Call clicked

Data to capture:

- Source page
- CTA clicked
- User state
- UTM source if available

---

## Success Criteria

The header is successful when:

- The top bar feels minimal and premium
- The menu does not feel crowded
- Users can access all pages easily
- Register / Sign In is visible
- Book a Strategy Call is always easy to find
- The navigation supports both consulting and platform behavior
