# User stories

**Traceability:** Q references point to the [requirements mapping](requirements-mapping.md), which maps the client questionnaire ([questionaire-hbl.md](questionaire-hbl.md)) to proposed needs and open questions. Check the source and status there before treating a proposal as confirmed.

## Shared acceptance checks

These checks apply to every story and page:

- Test the layout at viewport widths of 320, 768 and 1280 CSS pixels. At each width, page content and controls remain available without horizontal page scrolling or overlapping content.
- Every informative image has a meaningful text alternative; decorative images have an empty alternative. Keyboard users can reach and operate interactive controls, with a visible focus indicator.
- Text contrast meets WCAG AA: at least 4.5:1 for normal text and 3:1 for large text. Meaningful control boundaries and states have at least 3:1 contrast against adjacent colours.
- Headings use a logical hierarchy and page content uses semantic HTML.
- Internal links lead to the intended page or section without a broken destination. External links open in a separate tab.

---

# User Story US01: Hero and about on homepage

**Requirement refs:** Q18, Q21
**Page:** Home
**Priority:** Must
**Depends on:** None

## Story
As a new visitor, I want to quickly see Lydia's work and learn who she is, so that I can decide whether her services may suit me.

## Acceptance criteria
1. Given a visitor opens the homepage, when it loads, then they see an approved hero image and a brief introduction to Lydia.
2. Given a visitor views the homepage transformation showcase, when they inspect an approved example, then the before and after images are identified as a pair.
3. Given a visitor uses a mobile device, when they view the homepage at the shared test widths, then the content remains readable and usable without horizontal scrolling or overlap.

## Dev notes
- Approach: Use an accessible hero image and homepage introduction. A manually navigated slideshow is an option if Lydia approves it and provides suitable images.
- Open questions / needs from Lydia: High-resolution hero images, a profile photo, and short bio copy. Confirm whether she wants a slideshow.
- Fallback: Use one approved static hero image until custom assets are available.

## Status
[In Progress]

## Evidence
Not yet recorded.
---


# User Story US02: Enquiry call to action on every page

**Requirement refs:** Q10, Q16, Q17
**Page:** Site-wide
**Priority:** Should
**Depends on:** US05

## Story
As a potential customer, I want to enquire about services from a simple call to action on every page, so that I can easily reach out to book an appointment or ask a question no matter which page I am browsing.

## Acceptance criteria
1. Given a visitor is on any page, when they view the site navigation, then Lydia's approved enquiry call to action is available.
2. Given a visitor activates the enquiry call to action, when the action completes, then they reach the enquiry form described in US05.
3. Given a visitor uses the site on a mobile device, when they use the navigation at the shared test widths, then the enquiry call to action remains reachable and does not obscure page content.

## Dev notes
- Approach: Add an "Enquire" link to the site-wide navigation. Confirm the final wording with Lydia.
- Open questions / needs from Lydia: Confirm CTA wording.
- Fallback: If the enquiry form is unavailable, provide a direct WhatsApp link.

## Status
[To Do]

## Evidence
Not yet recorded.
---




# User Story US03: Genuine client reviews

**Requirement refs:** Q13, Q22
**Page:** Reviews / Site-wide
**Priority:** Should
**Depends on:** None

## Story
As a potential customer, I want to see genuine client reviews, so that I build trust and can decide if this service is for me.

## Acceptance criteria
1. Given a visitor reaches the reviews section, when it loads, then the five reviews approved by Lydia are displayed with their original ratings where those ratings are available.
2. Given a visitor reads a displayed review, when they inspect its details, then the approved client attribution and hair service are shown where those details are available in the approved review.
3. Given a visitor views the reviews on a mobile device, when they use the site at the shared test widths, then every review remains readable without horizontal scrolling or overlap.

## Dev notes
- Approach: Feature the five reviews approved by Lydia and provide a separate page for the full selection.
- Lydia's feedback: Approved five reviews to feature (Carlie Louise, Roxie Clarke, Lucy Stephenson, Khadija Torkhani, Melissa Sims). Permission to publish is confirmed.
- Open questions / needs from Lydia: Check that the approved review sources include the ratings and service details required by the acceptance criteria; do not invent missing details.
- Fallback: None.

## Status
[In Progress]

## Evidence
Not yet recorded.
---

# User Story US04: Gallery with before and afters

**Requirement refs:** Q13, Q21
**Page:** Gallery
**Priority:** Must
**Depends on:** None

## Story
As a potential customer, I want to browse examples of Lydia's work, so that I can assess the quality of her coloring and styling before enquiring about a home visit.

## Acceptance criteria
1. Given a visitor navigates to the gallery page, when it loads, then a grid of Lydia-approved hair transformation images is displayed.
2. Given a visitor views a gallery image, when they inspect it, then its description identifies the work and the image is not cropped in a way that hides the hairstyle. Approved before-and-after pairs are labelled as pairs.
3. Given a visitor browses the gallery on a mobile device, when they use the site at the shared test widths, then images keep their proportions and the gallery has no horizontal scrolling or overlap.

## Dev notes
- Approach: Instagram API, subject to testing.
- Lydia's feedback: Prefers recent Instagram posts if practical. A separately updated gallery is acceptable. Wants to approve photos before they go on the site. Photos updated about once a month. Permission to use client photos on the website is confirmed.
- Open questions / needs from Lydia: Confirm whether she wants before-and-after pairs in the gallery.
- Fallback: Hand-built gallery.

## Status
[To Do]

## Evidence
Not yet recorded.
---


# User Story US05: Enquiry form

**Requirement refs:** Q13, Q18
**Page:** Contact
**Priority:** Must
**Depends on:** None

## Story
As a client interested in this service, I want to enquire about particular questions and possible consultation and booking for services, so that I can secure a convenient home appointment and discuss my specific hair goals directly with Lydia.

## Acceptance criteria
1. Given a user opens the enquiry form, when it renders, then fields for name, required phone number, home address, and message/questions are present and marked as required, and an email field is available but optional.
2. Given a user submits a valid enquiry, when the form successfully processes it, then the user sees a confirmation that Lydia aims to reply within one working day. If the user provided an email address, an automatic acknowledgement is sent to that address.
3. Given a user leaves a required field blank or enters invalid data, when they submit the form, then validation identifies the problem and prevents invalid data from being processed.
4. Given the form cannot send an enquiry, when an error occurs, then the user is told the enquiry was not sent and is offered an alternative contact method.

## Dev notes
- Approach: A form with required fields that sends an email to Lydia.
- Lydia's feedback: Add the client's address. Phone number is required. Wants an automatic acknowledgement sent to the client. Photos are sent later by WhatsApp, not attached. Site can say she replies within one working day.
- Open questions / needs from Lydia: The required phone field and email field are confirmed. Lydia's receiving email address will be provided when needed and is not included in this document.
- Fallback: If the form cannot submit, show a clear error and a WhatsApp contact link. Do not show a success message or imply that an acknowledgement was sent.

## Status
[To Do]

## Evidence
Not yet recorded.
---

# User Story US06: Services and prices in one click

**Requirement refs:** Q6, Q7, Q13
**Page:** Services & Prices
**Priority:** Should
**Depends on:** None

## Story
As a visitor, I want finding services and prices to be as simple as one click, so that I can instantly check her mobile hair rates and service options without having to dig through confusing menus.

## Acceptance criteria
1. Given a visitor is on any page, when they activate the "Services & Prices" navigation link, then they reach the dedicated pricing page.
2. Given a visitor views the services and price list, when it loads, then each listed service has its description and "from" price, no service duration is shown, and coverage is stated as Banbury and surrounding villages.
3. Given a visitor browses pricing on a mobile device, when they use the site at the shared test widths, then all rates and service categories remain readable without horizontal scrolling or overlap.

## Dev notes
- Approach: Full price list and services available from every page in the nav bar, one click.
- Lydia's feedback: Prices are ready to provide. Show "from" prices, not service durations. Prices updated about once a year or less. Extra travel costs may apply and will be discussed before confirming. Coverage wording is "Banbury and surrounding villages". Do not state "no minimum booking".
- Open questions / needs from Lydia: None.
- Fallback: None.

## Status
[To Do]

## Evidence
Not yet recorded.
---

# User Story US07: Cancellation policy and deposits

**Requirement refs:** Q12
**Page:** FAQ
**Priority:** Should
**Depends on:** None

## Story
As a visitor, I want to understand Lydia's cancellation policy and deposit scheme before enquiring, so that I know her booking terms and financial requirements upfront with complete clarity before reaching out.

## Acceptance criteria
1. Given a visitor navigates to the FAQ page, when they view the policy section, then it states only information confirmed for publication.
2. Given the cancellation or deposit terms are not confirmed for publication, when a visitor views the FAQ page, then those terms are not presented as settled policy.
3. Given a visitor reads the policy on a mobile device, when they use the site at the shared test widths, then the content remains readable without horizontal scrolling or overlap.

## Dev notes
- Approach: Make the FAQ available from the site-wide navigation and footer.
- Lydia's feedback: Deposit "may be required upon booking". No further deposit details given.
- Open questions / needs from Lydia: Resolve a source discrepancy before publishing: the Q12 questionnaire mapping records cancellation terms, while this story's earlier feedback says the cancellation policy was not covered. Confirm the approved terms with Lydia, including deposit details.
- Fallback: Do not invent or publish unconfirmed policy terms.


## Status
[To Do]

## Evidence
Not yet recorded.
---

# User Story US08: Lydia's training

**Requirement refs:** Q5, Q13, Q22
**Page:** About
**Priority:** Should
**Depends on:** None

## Story
As a visitor thinking of using Lydia's services, I want to see what training she has done, so that I can trust the services on offer.

## Acceptance criteria
1. Given a visitor navigates to the About page, when they view the background section, then Lydia's confirmed training, qualifications, and professional background are presented.
2. Given Lydia has not confirmed a training or qualification detail, when the About page is published, then that unconfirmed claim is not included.
3. Given a visitor views the About page on a mobile device, when they use the site at the shared test widths, then the text remains readable without horizontal scrolling or overlap.

## Dev notes
- Approach: Create a separate About page with Lydia's background, training, and qualifications.
- Open questions / needs from Lydia: Ask for her training, qualifications, and professional background.
- Fallback: Do not make claims about qualifications that Lydia has not confirmed.

## Status
[To Do]

## Evidence
Not yet recorded.
---

# User Story US09: Social media and contact links

**Requirement refs:** Q16
**Page:** Site-wide
**Priority:** Should
**Depends on:** None

## Story
As a visitor, I want to easily find Lydia's social media links and reach out that way, so that I can contact her without using email.

## Acceptance criteria
1. Given a visitor is browsing any page, when they view the site-wide footer or contact section, then direct links to Lydia's approved Instagram, Facebook, and WhatsApp accounts are available.
2. Given a visitor activates a social media or WhatsApp link, when the action completes, then it opens the corresponding platform in a separate tab.
3. Given a visitor uses the social links on a mobile device, when they use the site at the shared test widths, then each link is operable without horizontal scrolling or overlap.

## Dev notes
- Approach: Show social and contact links in the site-wide footer and contact section.
- Lydia's feedback: WhatsApp 07956426536. Instagram: hairbylydiamai. Facebook: Hair by Lydia. Lydia's email address has been provided privately and is withheld from this document for privacy reasons. Any contact method can be shown most prominently.
- Open questions / needs from Lydia: Confirm whether Lydia's email address may be published as a contact link.
- Fallback: None.

## Status
[To Do]

## Evidence
Not yet recorded.

---