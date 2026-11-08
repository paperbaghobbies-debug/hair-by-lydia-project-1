# Hair by Lydia Readme.d (V1)

## Project purpose
Hair by Lydia is a home-visit hairdressing service covering Banbury and surrounding villages. The website should build trust and make it easy for visitors to enquire. 
Lydia wants visitors to see her work, meet her, and find clear ways to enquire, view the gallery, and see services and prices. My design approach is to introduce Lydia and her work before guiding visitors towards an enquiry. 
The site should feel professional and work well on phones, tablets and desktops.

## Research and Principles

I began by sending Lydia a questionnaire to understand her business, audience,
preferred style and what she needed from the website. I mapped her answers to
requirements, features and open questions, then recorded her follow-up
feedback to help clarify those needs.

I compared three of lydia's listed competitors and began looking at their layouts, galleries,
prices, enquiry routes, mobile experience and accessibility. I also researched
options for features such as the enquiry form, reviews, gallery, hosting and
content updates. These comparisons helped me consider what would work for
Lydia’s business rather than choosing features on appearance alone.

Using the questionnaire, feedback and research, I developed user stories and
acceptance criteria to connect client needs with planned features. I then
considered design principles and accessibility and created mobile and desktop
wireframes. Together, this work informed the website brief and its focus on
building trust and making enquiries straightforward.

I researched single-page applications and JavaScript-based templating alongside
a multi-page HTML approach. I decided to use separate HTML pages with the main
content included in the HTML, using JavaScript where needed for interactive
features. This gives important content a clear URL and makes it available
without relying on JavaScript rendering. It also supports my plan for clear
page titles, headings and links that search engines can follow.

This approach supports search engine optimisation (SEO), but does not guarantee
search rankings. A JavaScript-based site can also be indexed when implemented
correctly. 

I am using an Agile-inspired approach while not limitinig myself and my learning.I attempt to organising work into sprints and
individual cards with acceptance criteria and a Definition of Done. Sprint 0
focuses on planning and design; later work will involve building, testing and
deployment. I will review progress, record evidence and carry unresolved
questions forward as the project develops.


Lydia responded positively to the brief on 6 November 2026; see the
[review record](./docs/brief.md#9-review-and-sign-off). Some decisions—including enquiry
privacy details and hosting—still need confirmation.

### Planning and research documents

- [Client questionnaire](./docs/questionaire-hbl.md)
- [Requirements mapping](./docs/requirements-mapping.md)
- [Lydia’s feedback](./docs/lydia-feedback.md)
- [Competitor research](./docs/competitor-research.md)
- [Feature research and decisions](./docs/feature-research.md)
- [User stories](./docs/user-stories.md)
- [Design principles and accessibility](./docs/design-principles-accessibility.md)
- [Wireframes](./docs/wire-frames.md)
- [Website brief](./docs/brief.md)
- [Sprint 0 plan](./sprints/sprint-0.md)

## Value and audience

- Local people looking for a trusted home-visit hairdresser, mostly on mobile.
- Visitors arriving from Instagram, Facebook, WhatsApp and word of mouth.
- Clients who need reassurance about prices, travel, deposits and response times.

See the [user stories](./docs/user-stories.md),
[competitor research](./docs/competitor-research.md) and
[Lydia’s feedback](./docs/lydia-feedback.md) for the needs and research
informing the website’s value and audience.

## Features and pages

The website is planned to include the following pages:

- **Home:** An introduction to Lydia, a slideshow of her work and featured reviews.
- **Services & Prices:** Services, “from” prices, and travel and deposit information.
- **Enquiry:** A form and contact options for asking about appointments.
- **Reviews:** Client reviews approved by Lydia.
- **Gallery:** Photos of Lydia’s work. The approach to Instagram content is still to be confirmed.
- **FAQ:** Answers about cancellation, deposits and other common questions.
- **404:** Explains that the page could not be found and provides a link back to the home page.


```text
MOBILE                                           DESKTOP
+----------------------------------------------+  +------------------------------------------------------------------------------------+
| ✱ Hair By Lydia →        [ Enquire ] [ Menu ]|  | ✱ Hair By Lydia → Home → Services and Prices → Gallery → Reviews → FAQ → [Enquire] |
+----------------------------------------------+  +------------------------------------------------------------------------------------+
|                 HERO SLIDE                   |  |                                    HERO SLIDE                                      |
| +------------------------------------------+ |  |                         Featured work image (alt text)                             |
| | Featured work image (alt text)           | |  |                            [ ← ] [ ▶ ] [ ❚❚ ] [ → ]                                |
| +------------------------------------------+ |  |                              H1 Hair by Lydia                                      |
|         [ ← ] [ ▶ ] [ ❚❚ ] [ → ]            |  |                         Short intro line (paragraph)                                |
|              H1 Hair by Lydia                |  +------------------------------------------------------------------------------------+
|          Short intro line (paragraph)        |  |                                 H2 About Lydia                                     |
+----------------------------------------------+  |                                                                                    |
|              H2 About Lydia                  |  |               +---------+     H3 What Lydia does                                  |
|                                              |  |               |  Photo  |     About text (paragraph)                              |
|  +---------+    H3 What Lydia does           |  |               | (Lydia) |                                                         |
|  |  Photo  |    About text (paragraph)       |  |               +---------+                                                         |
|  | (Lydia) |                                 |  |                  Not sure what to book? [ Ask Lydia → ]                           |
|  +---------+                                 |  |                    [ Gallery ] [ Services ] [ Enquire ]                           |
|  Not sure what to book? [ Ask Lydia → ]      |  +------------------------------------------------------------------------------------+
|    [ Gallery ] [ Services ] [ Enquire ]      | |                             H2 What clients say                                    |
+----------------------------------------------+  |                             Review text (paragraph)                                |
|           H2 What clients say                |  |                             Reviewer name                                          |
|           Review text (paragraph)            |  |                      [ ← ] [ ❚❚ ] 1 of 5 [ → ]                                      | 
|           Reviewer name                      |  |                             Read all reviews →                                     |
|      [ ← ] [ ❚❚ ] 1 of 5 [ → ]               |  +-----------------------------------------------------------------------------------+
|           Read all reviews →                 |  | • Home →               • Gallery →                                      (IG)       |
+----------------------------------------------+  | • Services + Prices →  • Reviews →                                      (FB)       |
| • Home →              • Gallery →    (IG)    |  | • Enquire →            • FAQ →                                          (WA)       |
| • Services + Prices → • Reviews →    (FB)    |  |                                                                                    |
| • Enquire →           • FAQ →        (WA)    |  | Hair by Lydia                                                                      |
|                                              |  | Rights etc.                                                                        |
| Hair by Lydia                                |  +------------------------------------------------------------------------------------+
| Rights etc.                                  |
+----------------------------------------------+
```

See the [wireframes](./docs/wire-frames.md) for the planned page layouts.

The website is planned to include the following features:

- **Responsive layout:** Designed for phones, tablets and desktops.
- **Shared navigation:** Links to the main pages, with an enquiry call to action.
- **Hero slideshow:** Featured photos of Lydia’s work, with navigation and pause controls.
- **Review carousel:** Approved client reviews with previous, next and pause controls.
- **Enquiry form:** Collects contact details and an enquiry, with validation and an alternative contact method if sending fails.
- **Email acknowledgement:** Sent after a successful enquiry when the visitor provides an email address.
- **Gallery:** Displays photos of Lydia’s work on Instagram. Custom gallery will be built as fallback 
- **Contact and social links:** Links to Lydia’s contact and social media channels.
- **Accessibility:** Planned support for keyboard navigation, visible focus, meaningful image descriptions and readable contrast.

The site will also have shared navigation and an enquiry call to action across its pages.
See the [feature research](./docs/feature-research.md) and [design principles and accessibility](./docs/design-principles-accessibility.md)
for the research and design decisions informing these features.

## Design and accessibility

The planned design aims to feel warm, personal and trustworthy, using
approved photos of Lydia’s work.

- **Colour palette:** Taupe (`#7F7367`), cream (`#FAF3EB`), dark brown
  (`#342B24`) and muted gold (`#C6A15B`), approved by Lydia.
- **Typography:** Noto Serif Display Extra Condensed and Luxurious Script
  for branding. Lato is proposed for body text, pending Lydia’s confirmation.
- **Layout:** A mobile-first, multi-page design with a clear enquiry action
  in the navigation.
- **Header:** A taupe header fixed at the top, rather than a transparent
  header, following Lydia’s feedback.
- **Accessibility:** The design plans for meaningful image descriptions,
  keyboard navigation, visible focus, sufficient contrast and labelled form
  fields. WCAG 2.2 AA is the working target, pending confirmation against
  the assignment brief.

See the [design principles and accessibility checklist](./docs/design-principles-accessibility.md)
and [wireframes](./docs/wire-frames.md) for further details.

## Testing

Testing is planned throughout development. This section will summarise the
checks performed, results, issues and retests.

**Test plan:** To be created. It will link tests to user stories and record
steps, expected and actual results, status, and bug or fix notes.

## Deployment

The hosting provider and domain are not yet confirmed. This section will
include the live site link and deployment steps once they have been verified.

## Credits

- **Lydia:** Client questionnaire responses, feedback, branding and project
  requirements.
- **Research sources:** Guidance from MDN, Google, W3C, Nielsen Norman Group
  and Laws of UX helped inform the planning and design. Full source links are
  in the [feature research](./docs/feature-research.md) and
  [design principles](./docs/design-principles-accessibility.md).
- **Competitor websites:** Hairnovate, Emz Hair & Wellness and Matthew Grant
  Hairdressing were reviewed for research and inspiration. See the
  [competitor research](./docs/competitor-research.md).
- **Learning resources:** freeCodeCamp, W3Schools and Code Institute for
  resources that informed my understanding of coding and web development.
- **Project management:** The [Agile Manifesto](https://agilemanifesto.org/)
  informed my Agile-inspired approach to planning and reviewing work.
- **AI assistance:** Copilot and Claude have supported documented parts of
  the planning process. See the [AI log](./docs/ai_log.md) and
  [AI disclosure](./docs/appendix.md) for details.