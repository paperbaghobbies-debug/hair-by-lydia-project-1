# Hair by Lydia: Website Brief

**Date:** 5 November 2026

**Status:** Prepared for Lydia's review; not yet signed off

**Source key**

- **[Q]** Lydia's questionnaire or feedback, including my recollection of our conversation where noted.
- **[P]** My proposal, interpretation or design decision.
- **[C]** To confirm or verify.

**Sources:** [Questionnaire](./questionaire-hbl.md), [Lydia's feedback](./lydia-feedback.md), [user stories](./user-stories.md), [feature research](./feature-research.md), [competitor research](./competitor-research.md), [wireframes](./wire-frames.md), [design principles and accessibility](./design-principles-accessibility.md), [requirements mapping](./requirements-mapping.md), and my [original rough notes](../brief-rough-note.txt).

## 1. Purpose

Hair by Lydia is a home-visit hairdressing service covering Banbury and surrounding villages. The website should build trust and make it easy for visitors to enquire. **[Q]**

Lydia wants visitors to see her work, meet her, and find clear ways to enquire, view the gallery, and see services and prices. My design approach is to introduce Lydia and her work before guiding visitors towards an enquiry. **[Q/P]**

The site should feel professional and work well on phones, tablets and desktops. **[P]**

### Success measures

- **Client outcome [Q]:** Lydia receives more enquiries and bookings from new clients who found her online.
- **Proposed usability targets [P]:** A new visitor can reach each page within three clicks and can view Lydia's work, prices and reviews and send an enquiry in under two minutes on a phone. These are goals, not requirements that should make design harder; I will check them against the project specification and validate them through mobile usability testing.
- Lydia can keep the site current through a low-effort process of sending me updates to publish. **[Q]**

## 2. Audience

- Local people looking for a trusted home-visit hairdresser, mostly on mobile.
- Visitors arriving from Instagram, Facebook, WhatsApp and word of mouth.
- Clients who need reassurance about prices, travel, deposits and response times.

## 3. Scope and schedule

The project target deadline is **25 December 2026**. If needed, work may continue through **1 January 2027** as a grace period. **[P]**

- **Sprint 0 — planning:** Prepare this brief for client review, with researched feature decisions, user stories and wireframes.
- **Sprint 1 — build:** Create the shared layout and navigation, Home, Services & Prices, Enquiry, Reviews, Gallery and FAQ pages; implement form validation; add Lydia's approved content; and write a README.
- **Sprint 2 — test, deploy and document:** Complete responsive and accessibility checks, record manual test procedures and results, deploy with the domain, capture screenshots, prepare lifecycle documentation and a handover guide for content updates, and check the site against the specification.
- Keep time before the deadline for fixes and submission checks; use the grace period only if needed.

### Out of scope

- Online booking, payments and deposit handling. Lydia consults clients and manually confirms appointments; the site will explain that a deposit may be required upon request.
- A self-service CMS and post-project maintenance. Lydia prefers to send updates for me to publish.
- Photo uploads through the enquiry form. Clients will send photos later by WhatsApp.
- Service durations. The price list will use “from” prices.
- Stating that there is no minimum booking. Lydia confirmed there is no minimum booking, but the current decision in US06 is not to state this on the site.

### Main risks and checks

- Whether displaying recent Instagram posts is practical.
- Getting Lydia's preferred and approved hero and About-section images in time.
- Verifying domain, hosting, form-service and content-update costs before launch.
- Gathering testing and deployment evidence throughout the project rather than leaving it until the end.

## 4. Content and update plan

### Received or confirmed by Lydia

| Item | Planned use | Notes |
|---|---|---|
| Logo and brand files | All pages | |
| Brand fonts | All pages | Use as specified below. |
| Contact links | Site-wide and Enquiry | WhatsApp, Instagram, Facebook and email; do not expose private contact details in public project files without permission. |
| Service area | Home and FAQ | “Banbury and surrounding villages.” |
| Services and “from” prices | Services & Prices (US06) | No service durations. |
| Travel wording | Services & Prices and FAQ | Extra costs may apply depending on location and will be discussed before confirmation. |
| Deposit wording | Services & Prices and FAQ | Deposits may be required upon request. |
| Five reviews | Reviews and Home (US03) | Lydia has approved their use. Check original sources for ratings and service details; do not invent missing information. |
| Cancellation terms | FAQ (US07) | Confirmed terms are recorded in section 5. |

### Still to supply, select or prepare

| Item | Planned use | Owner | Next step |
|---|---|---|---|
| Preferred, high-resolution hero images | Home slideshow (US01) | Lydia | Lydia to choose/provide the images and approve their use. |
| Preferred About-section image and short bio | Home (US01, US08) | Lydia | Ask Lydia which image and details she wants included. |
| Gallery photos | Gallery (US04) | Lydia | Lydia approves every photo before publication. Use a hand-built gallery if Instagram display is impractical. |
| Intro line and enquiry button wording | Home and site-wide (US02) | Me, with Lydia's approval | Draft and ask Lydia to approve. |
| Image alt text | Home and Gallery | Me, with Lydia's review | Write descriptive alt text for the selected images. |
| Enquiry fields and privacy notice | Enquiry (US05) | Me and Lydia | Use a required phone field and optional email. Confirm what location detail is needed and the privacy/data-handling details before implementation. |
| FAQ questions and answers | FAQ (US07) | Me, with Lydia's approval | Draft the confirmed cancellation and deposit wording. Do not invent late-arrival terms. |

Lydia expects photos to be updated about monthly and prices about once a year or less. She will send updates for me to publish. **[Q]**

### Content rules

- Lydia approves all gallery photos and copy I write before it goes live.
- Do not put Lydia's WhatsApp number or client photos in a public repository unless she agrees.
- Set image dimensions and file-size limits so the site remains fast on mobile. **[P]**
- Track content through: Not requested → Requested → Received → Approved → Published. **[P]**

## 5. Features and decisions

### Enquiry

- The form will collect a name, required phone number, optional email address, and a short description or question. **[Q]**
- Include a location/address field only after confirming the necessary level of detail and whether it is required. Agree the privacy notice and data-handling details before collecting personal information. **[C]**
- Include an optional “How did you hear about Lydia?” dropdown with word of mouth, Google/search, Instagram, Facebook, other, and prefer not to say. Include the answer in the enquiry email only; do not add tracking. **[P]**
- If a client provides an email address, send an automatic acknowledgement after a successful submission. **[Q]**
- Lydia aims to reply within **two working days**. This reflects my conversation with Lydia; that conversation is not separately recorded. **[Q, as recalled by me]**
- Make clear that an enquiry is not a confirmed booking. Lydia consults with the client and confirms the service and appointment manually. **[Q]**
- If the form cannot send, say the enquiry was not sent and offer another contact method. **[P]**

The enquiry story currently tracks the location and privacy/data-handling details as implementation blockers. See [US05](./user-stories.md#user-story-us05-enquiry-form).

### Reviews

- Feature the five reviews Lydia approved in a slowly rotating carousel on the Home page, with previous/next and pause/resume controls that keyboard users can operate.
- This carousel behaviour is my design choice, informed by competitor research and the style I want. Keep reviews readable without JavaScript and provide text alternatives for star ratings.
- Reuse the reviews as cards on the separate Reviews page. Google Reviews integration is not planned.
- Check the original ratings and service details against the approved review sources; do not invent missing information. **[C]**

### Gallery and About content

- Lydia prefers recent Instagram posts if practical. **[Q]**
- If Instagram display is not practical, I will build a hand-updated gallery using photos Lydia approves. **[P]**
- The About content belongs on the Home page; there will not be a separate About page. This follows Lydia's request and the current user-story plan. **[Q/P]**
- Lydia will choose/provide her preferred images for the hero slideshow and About section. **[C]**

### Cancellation and deposits

- **Cancellation terms [Q]:** No fee with at least two days' notice; 50% of the booked service cost with one day's notice; 100% for same-day cancellation or no-show.
- Outstanding cancellation fees must be paid in full before future appointments can be booked or confirmed. **[Q]**
- Deposits may be required upon request. The amount, payment method and refund terms are unspecified; do not invent them. **[Q]**
- No late-arrival terms have been provided. The FAQ must not invent a late-arrival policy. **[C]**

### Domain, hosting and content updates

- Lydia owns and pays for the domain. Her preferred domain name is Hairbylydia-Banbury; availability needs checking. **[Q/C]**
- Cloudflare Pages is a researched hosting option, not a confirmed choice. Verify current terms, compatibility and costs before launch. **[P/C]**
- Do not build a self-service content update feature. Agree a simple update process and verify related costs and turnaround before choosing the ongoing arrangement. **[P/C]**

## 6. User stories

| ID | Story | Page | Priority | Status |
|---|---|---|---|---|
| [US01](./user-stories.md#user-story-us01-hero-and-about-on-homepage) | Hero and About on homepage | Home | Must | In progress |
| [US02](./user-stories.md#user-story-us02-enquiry-call-to-action-on-every-page) | Enquiry call to action on every page | Site-wide | Should | To do |
| [US03](./user-stories.md#user-story-us03-genuine-client-reviews) | Genuine client reviews (carousel plus full page) | Reviews / site-wide | Should | In progress |
| [US04](./user-stories.md#user-story-us04-gallery-with-before-and-afters) | Gallery with before and afters | Gallery | Must | To do |
| [US05](./user-stories.md#user-story-us05-enquiry-form) | Enquiry form | Home / Contact | Must | Blocked: location and privacy/data-handling details |
| [US06](./user-stories.md#user-story-us06-services-and-prices-in-one-click) | Services and prices in one click | Services & Prices | Should | To do |
| [US07](./user-stories.md#user-story-us07-cancellation-policy-and-deposits) | Cancellation policy and deposits | FAQ | Should | To do |
| [US08](./user-stories.md#user-story-us08-lydias-training) | Lydia's training | Home (About section) | Should | To do |
| [US09](./user-stories.md#user-story-us09-social-media-and-contact-links) | Social media and contact links | Site-wide | Should | To do |

The [user stories](./user-stories.md) contain full acceptance criteria, development notes and evidence. Shared checks include testing at 320, 768 and 1280 px; alt text; keyboard use; WCAG AA contrast; semantic headings; and working links.

## 7. Design direction

- **Feel:** Warm, personal, uncluttered and trustworthy, with real photos of Lydia's work. **[Q]**
- **Palette:** Taupe `#7F7367`, Cream `#FAF3EB`, Dark brown `#342B24`, and Muted gold `#C6A15B`. Lydia approved this palette on 29 October 2026. **[Q]**
- **Typography:** Use Noto Serif Display Extra Condensed for “Hair by Lydia” branding and Luxurious Script for other branding. Lato is my proposed body font and still needs Lydia's confirmation. **[Q/P/C]**
- **Layout:** Mobile-first, separate pages, and a clear enquiry action in the site-wide navigation. **[P]**
- **Accessibility:** Use alt text, keyboard navigation, visible focus, sufficient contrast and labelled form fields. The working target is WCAG 2.2 AA, pending confirmation against the assignment brief. See the [accessibility checklist](./design-principles-accessibility.md).
- **Hero:** Lydia requested a slideshow of her featured work, with controls to move between slides and pause/resume. Use approved images. **[Q]**
- **Header:** Use a taupe header fixed from the top of the page, rather than a transparent header. Lydia agreed to this direction on 28 October 2026 because her logo would not blend into a transparent bar. **[Q]**
- **Wireframes:** See [wire-frames.md](./wire-frames.md) for the key mobile and desktop pages.

### Palette contrast checks

The following checks are recorded in the wireframes. Check final rendered combinations, including hover, active and keyboard-focus states, in the built site.

| Combination | Contrast ratio | Recorded result |
|---|---:|---|
| White on taupe | 4.61:1 | Passes AA for normal text |
| Dark brown on cream | 12.58:1 | Passes AAA |
| Dark brown on muted gold | 5.70:1 | Passes AA |

## 8. Constraints and outstanding checks

- Lydia owns and pays for the domain.
- Lydia prefers to send content updates rather than edit the site herself.
- Lydia's permission covers use of client photos on the website; still follow the separate rule not to place client photos in a public repository without agreement.
- Verify domain availability and hosting, form-service and content-update costs before committing to the launch setup.
- The main remaining content question is which images Lydia prefers for the hero slideshow and About section.
- Confirm whether recent Instagram posts can be used practically; use my hand-built gallery fallback if not.

Detailed enquiry-form location and privacy/data-handling requirements remain tracked in US05 and must be resolved before implementing that form.

## 9. Review and sign-off

This brief is prepared for Lydia's review. I will record the date sent, her feedback and any changes; I will mark it client-reviewed or signed off only when that evidence exists.

| Date | Reviewer | Outcome | Evidence |
|---|---|---|---|
| Pending | Lydia | Awaiting review | None yet |