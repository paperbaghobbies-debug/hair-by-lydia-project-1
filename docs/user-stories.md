# User stories

**Traceability:** Q references point to the [requirements mapping](requirements-mapping.md). The [completed questionnaire](questionaire-hbl.md) and [Lydia's feedback record](lydia-feedback.md) are the client records; the mapping is the student's analysis, not a separate client approval. Where the mapping and a direct client record appear to differ, use the direct client record and update the mapping/story. Keep unverified points open rather than treating proposals as confirmed.

**Status and priority:** “In Progress” includes research and planning, not only implementation. Add build and test evidence as development proceeds. “Must” stories are required before public launch; they do not all need to be completed in the first sprint.

## Coverage of key needs

| Need | Story or backlog | Status / trace |
|---|---|---|
| Consultation before booking | US05 | The enquiry is not a booking; Lydia consults before manually confirming the service and appointment. Confirm whether the form starts the online consultation or Lydia follows up separately (Q8, Q10). |
| Travel charges | US06 | The service-area and price information says extra travel charges may apply and will be discussed before confirmation (Q14–Q15; see the [requirements mapping](requirements-mapping.md)). |
| “Not sure what to book?” enquiries | US05 | Add a homepage prompt that routes unsure visitors to the enquiry form so they can ask for advice (Q13, Q18). |
| Ongoing content and domain costs | Sprint 1 carry-forward backlog | Verify domain registration/renewal, hosting, form/service and maintenance costs, plus the content-update process, before the build/launch decision (Q23–Q26; [Sprint 0 carry-forward backlog](../sprints/sprint-0.md#11-carry-forward-backlog-and-later-specification); [feature research](feature-research.md)). |

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
2. When a visitor opens the homepage, when the hero loads, then they see a slideshow of Lydia's approved featured work, with controls to move between slides and to pause and resume the slideshow.
3. When a visitor uses a mobile device, when they view the homepage at the shared test widths, then the content remains readable and usable without horizontal scrolling or overlap.

## Dev notes
- Approach: Use an accessible hero slideshow of Lydia's approved featured work, with a brief introduction and an About Lydia section on the homepage. Lydia requested the slideshow.
- Open questions / needs from Lydia: High-resolution hero images, a profile photo, and short bio copy.
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
**Page:** Home (featured carousel) and Reviews (full page)
**Priority:** Should
**Depends on:** None

## Story
As a potential customer, I want to see genuine client reviews, so that I build trust and can decide if this service is for me.

## Acceptance criteria
1. Given a visitor views the homepage, when the featured reviews carousel loads, then it displays the five reviews approved by Lydia, with their original ratings where those ratings are available.
2. Given a visitor navigates to the Reviews page, when it loads, then it displays the full selection of reviews Lydia has approved for publication.
3. Given a visitor reads a displayed review, when they inspect its details, then the approved client attribution and hair service are shown where those details are available in the approved review.
4. Given the homepage reviews carousel is active, when its interval elapses, then it advances slowly to the next review; visitors can pause and resume rotation, and keyboard users can operate the pause, previous and next controls.
5. Given a visitor views the homepage carousel or Reviews page on a mobile device, when they use the site at the shared test widths, then reviews remain readable without horizontal scrolling or overlap.

## Dev notes
- Approach: Feature the five reviews approved by Lydia in a slowly auto-rotating homepage carousel with accessible pause/resume and previous/next controls. Build the full approved selection on a separate Reviews page in its own page sprint. Slow rotation is the student's design choice, informed by competitor research and the desired style.
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
- Approach: Use Lydia's Instagram posts if technically practical; otherwise build a hand-updated gallery.
- Lydia's feedback: She controls which photos she publishes to Instagram and prefers recent posts if practical. Photos are updated about once a month. Permission to use client photos on the website is confirmed.
- The Instagram option remains subject to technical feasibility; Lydia's publishing control is the approval step for posts shown from her account.
- Open questions / needs from Lydia: Confirm whether she wants before-and-after pairs in the gallery.
- Fallback: Hand-built gallery.

## Status
[To Do]

## Evidence
Not yet recorded.
---


# User Story US05: Enquiry form

**Requirement refs:** Q8, Q10, Q13, Q17, Q18
**Page:** Home / Contact
**Priority:** Must
**Depends on:** None

## Story
As a client interested in this service, I want to enquire about a service or ask for advice if I am unsure what to book, so Lydia can understand my hair goals and consult with me before manually confirming the right service and appointment.

## Acceptance criteria
1. Given a visitor is unsure which service to book, when they view the homepage, then a “Not sure what to book?” prompt leads them to the enquiry form and invites them to describe their hair goals and current hair.
2. Given a user opens the enquiry form, when it renders, then fields for name, required phone number, a description/questions, and optional email are present. The form does not request an address or separate location.
3. Given Lydia receives an enquiry, when she considers a booking, then the site makes clear that the enquiry does not confirm a booking and that she consults with the client before manually confirming the service and appointment. Whether the form itself starts the online consultation or Lydia follows up separately remains to be confirmed.
4. Given a user submits a valid enquiry, when the form successfully processes it, then the user sees a confirmation that Lydia aims to reply within one working day. If the user provided an email address, an automatic acknowledgement is sent to that address.
5. Given a user submits personal information, when they review the form, then a concise privacy notice is available from the form and explains what information is collected, why, who receives or processes it, and the verified handling and retention/deletion approach. The notice is also reachable from the footer and FAQ.
6. Given a user opens the enquiry form, when it renders, then an optional "How did you hear about Lydia?" dropdown offers: word of mouth, Google/search, Instagram, Facebook, other, and prefer not to say. The selected answer is included in the enquiry email, and no backend tracking is added.
7. Given a user leaves a required field blank or enters invalid data, when they submit the form, then validation identifies the problem and prevents invalid data from being processed.
8. Given the form cannot send an enquiry, when an error occurs, then the user is told the enquiry was not sent and is offered an alternative contact method.

## Dev notes
- Approach: A form with required fields that sends an email to Lydia.
- Lydia's feedback: Phone number is required. The service area is Banbury and surrounding villages; no separate location or address field is needed. She wants an automatic acknowledgement sent to the client. Photos are sent later by WhatsApp, not attached. Site can say she replies within one working day.
- Before enabling submissions, verify the form provider and actual data handling, including who receives/processes data, access/protection, retention and deletion. Link the privacy information from the form and make it available in the footer and FAQ. Confirm whether the form is the online consultation's starting point or Lydia follows up separately. The required phone field and optional email field are recorded in the story; Lydia's receiving email address will be provided when needed and is not included here.
- Fallback: If the form cannot submit, show a clear error and a WhatsApp contact link. Do not show a success message or imply that an acknowledgement was sent.

## Status
[In Progress: form design can proceed; verify data handling before enabling submissions]

## Evidence
Service-area clarification: Banbury and surrounding villages. Verify provider and data-handling details before enabling submissions.
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
2. Given a visitor views the services and price list, when it loads, then each listed service has its description and "from" price, no service duration is shown, coverage is stated as Banbury and surrounding villages, and it explains that extra travel charges may apply depending on location and will be discussed before confirmation.
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
As a visitor, I want to understand Lydia's cancellation terms and when deposits may be requested, so that I know the confirmed booking conditions before enquiring.

## Acceptance criteria
1. Given a visitor navigates to the FAQ page, when they view the cancellation section, then it states that cancellations with at least 2 days' notice have no fee, cancellations with 1 day's notice incur 50% of the booked service cost, and same-day cancellations or no-shows incur 100%.
2. Given a visitor reads the policy, when they view the outstanding-fees condition, then it says outstanding cancellation fees must be paid in full before future appointments can be booked or confirmed.
3. Given a visitor reads the deposit information, when they view the FAQ, then it says deposits may be required upon request and does not invent an amount, payment method, refund rule or trigger.
4. Given a visitor looks for late-arrival terms, when no terms have been confirmed by Lydia, then the FAQ does not invent or imply a late-arrival policy.
5. Given a visitor reads the policy on a mobile device, when they use the site at the shared test widths, then the content remains readable without horizontal scrolling or overlap.

## Dev notes
- Approach: Make the FAQ available from the site-wide navigation and footer.
- Authoritative client record: Lydia's completed Q12 response in the [questionnaire](questionaire-hbl.md), also transcribed in the [feedback record](lydia-feedback.md), says the policy should be clearly displayed. The [requirements mapping](requirements-mapping.md) is a derived summary and does not contradict the client response; the earlier discrepancy note in this story was incorrect and is removed.
- Confirmed cancellation terms: no fee with at least 2 days' notice; 50% of the booked service cost with 1 day's notice; 100% for same-day cancellation or no-show; outstanding fees must be paid before future bookings are booked or confirmed. Communicate the terms in a friendly, clear way.
- Lydia's feedback on deposits: They may be required upon request; no amount, payment method, refund rule or trigger was provided.
- Open questions / needs from Lydia: Confirm whether the site should cover late arrivals, as Q12 asked about them but the response gives no late-arrival terms. Confirm any additional deposit details before adding them.
- Fallback: Publish only the cancellation terms above and the confirmed general deposit statement; do not invent missing terms.


## Status
[To Do]

## Evidence
[Q12 in the completed questionnaire](questionaire-hbl.md); [Lydia's feedback record](lydia-feedback.md); [derived requirements mapping](requirements-mapping.md).
---

# User Story US08: Lydia's training

**Requirement refs:** Q5, Q13, Q22
**Page:** Home (About Lydia section; the separate About page was dropped)
**Priority:** Should
**Depends on:** None

## Story
As a visitor thinking of using Lydia's services, I want to see what training she has done, so that I can trust the services on offer.

## Acceptance criteria
1. Given a visitor views the About Lydia section on the homepage, when they read the background content, then Lydia's confirmed training, qualifications, and professional background are presented.
2. Given Lydia has not confirmed a training or qualification detail, when the homepage is published, then that unconfirmed claim is not included.
3. Given a visitor views the About Lydia section on a mobile device, when they use the site at the shared test widths, then the text remains readable without horizontal scrolling or overlap.

## Dev notes
- Approach: Include Lydia's background, training, and qualifications in the About Lydia section on the homepage. The separate About page was dropped in favour of the homepage section.
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
- Lydia's feedback: Instagram: hairbylydiamai. Facebook: Hair by Lydia. Lydia's WhatsApp number and email address were provided privately and are withheld from this document for privacy reasons. Any contact method can be shown most prominently.
- Open questions / needs from Lydia: Confirm whether Lydia's email address may be published as a contact link.
- Fallback: None.

## Status
[To Do]

## Evidence
Not yet recorded.

---