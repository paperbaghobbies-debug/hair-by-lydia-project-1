# Wireframes – Hair by Lydia

**Status:** Draft (hand notes → wireframes)
**Sources:** hand-drawn notes in `docs/screenshots/handnote/`
**Last updated:** 2026-11-05
**Scope note (US08):** There is no separate About page wireframe. About content is built into the homepage (H2 About section with Lydia's photo and intro), so US08 is covered there.
**Scope note (tablet, 768px):** No separate tablet wireframes. At 768px the mobile layout is reused with wider content, and the desktop layout takes over once the full navigation fits on one line. This will be checked when the page is built, at the shared test widths of 320, 768 and 1280px.
**Scope note (detail):** These wireframes show layout only. Final copy, prices and styling will be added at build time, following the user stories.

## Design notes (Passes 1.2 and 1.5)

> **To do:** the README has not been created yet. When it is, copy this section into it under a "UX design" heading, together with the design-decision notes.

### Colours

Palette from Lydia's logo and Q20 feedback ([lydia-feedback.md](./lydia-feedback.md)). Ratios checked against the WebAIM formula; evidence in [feature-research.md](./feature-research.md#11-colour-palette-and-contrast).

| Colour | Hex | Use | Pairing | Contrast | Result |
|---|---|---|---|---:|---|
| Taupe | `#7F7367` | Header and navigation bar | White `#FFFFFF` text | 4.61:1 | AA normal text |
| Cream | `#FAF3EB` | Page background | Dark brown `#342B24` text | 12.58:1 | AAA normal text |
| Dark brown | `#342B24` | Body text, headings, focus outline on cream | Cream background | 12.58:1 | AAA |
| Muted gold | `#C6A15B` | Call-to-action buttons and button states | Dark brown `#342B24` text | 5.70:1 | AA normal text |
| White | `#FFFFFF` | Text and focus outline on taupe or dark brown | Dark brown `#342B24` background | 13.84:1 | AAA |
| Deep red | `#8B1E1E` | Form error messages | Cream background | 8.29:1 | AAA |
| Deep green | `#2E5D34` | Form success messages | Cream background | 6.99:1 | AAA |

Rules:
- Gold on cream is only 2.21:1 and taupe on cream is 4.19:1, so neither is used as text. A gold button must keep dark-brown text, and its edge must not be the only thing that marks it as a button.
- Error and success colours are always paired with an icon and text, never colour alone (Pass 1.2).
- Keyboard focus: a 3px dark-brown outline on cream, and a white outline on the taupe header. Check hover, active and focus states in the built page.
- Hero text sits below the hero image, not over it, so the foreground text is never competing with a photo (Pass 1.4).
- Check the error and success ratios again in the WebAIM Contrast Checker once the final colours are set.

### Fonts

| Role | Font | Used for | Status |
|---|---|---|---|
| Brand and headings | Noto Serif Display (Extra Condensed) | Logo text, H1 and H2 headings | Chosen by Lydia (Q20) |
| Decorative accents | Luxurious Script | Branding flourishes only, not body text, navigation or forms | Chosen by Lydia (Q20) |
| Body | Lato | Paragraphs, navigation, forms, buttons | Proposed by me. To confirm with Lydia |

| Element | Size (desktop) | Mobile |
|---|---|---|
| Body text | 1rem (16px) minimum | 1rem |
| H1 | 2.5rem | Scales down, never below 2rem |
| H2 | 2rem | 1.75rem |
| H3 | 1.5rem | 1.25rem |

Line height is 1.5 for body text. Sizes use `rem` so the text scales with the user's browser settings.

### Alt-text rules

1. Gallery and hero images describe the hairstyle, for example "Layered auburn bob, side view".
2. Before/after pairs say which is which, for example "Before: shoulder-length brown hair" and "After: ...".
3. Lydia's photo: "Lydia, hairdresser, smiling".
4. Decorative images use an empty `alt=""`.
5. The logo link reads "Hair by Lydia – home".
6. Social icons are named by platform, for example "Instagram (opens in new tab)".

## Home Page

**Goal:** Show visitors who Lydia is and what she does as soon as they land.
**Source:** [homepagehandnote.jpg](./screenshots/handnote/homepagehandnote.jpg)
**Status:** Sketched

### Hand note
![Home page hand note](./screenshots/handnote/homepagehandnote.jpg)

### Wireframe - Homepage Mobile (US01,US03,US09)

```text
+------------------------------------------------+
| ✱ Hair By Lydia →          [ Enquire ] [ Menu ]|
+------------------------------------------------+
|                  HERO SLIDE
| +--------------------------------------------+ |
| |   Featured work image (alt text)           | |
| +--------------------------------------------+ |
|            [ ← ]  [ ▶ ]  [ ❚❚ ]  [ → ]         |
|            H1  Hair by Lydia                   |
|        Short intro line (paragraph)            |
+------------------------------------------------+
|             H2  About Lydia                    |
|                                                |
|     +----------+      H3  What Lydia does      |
|     |  Photo   |      About text (paragraph)    |
|     | (Lydia)  |                                |
|     +----------+                               |
|    Not sure what to book? [ Ask Lydia → ]      |
|      [ Gallery ] [ Services ] [ Enquire ]      |
+------------------------------------------------+
|             H2  What clients say               |
|           Review text (paragraph)              |
|           Reviewer name                        |
|   [ ← ]    [ ❚❚ ]   1 of 5    [ → ]            |
|          Read all reviews →                    |
+------------------------------------------------+
| • Home →               • Gallery →     (IG)    |
| • Services + Prices →  • Reviews →     (FB)    |
| • Enquire →            • FAQ →         (WA)    |
|                                                |
| Hair by Lydia                                  |
| Rights etc.                                    |
+------------------------------------------------+
```
### Wireframe - Mobile Menu Open
```text
+------------------------------------------------+
| ✱ Hair By Lydia →          [ Enquire ] [ Close]|
+------------------------------------------------+
| • Home →                                       |
| • Services and Prices →                        |
| • Gallery →                                    |
| • Reviews →                                    |
| • FAQ →                                        |
+------------------------------------------------+
```
### Wireframe - Homepage Desktop (US01,US03,US09)
```text
+--------------------------------------------------------------------------------------+
| ✱ Hair By Lydia →   Home →  Services and Prices →  Gallery →  Reviews →  FAQ → [Enquire] |
+--------------------------------------------------------------------------------------+
|                                     HERO SLIDE                                       |
|                          Featured work image (alt text)                              |
|                             [ ← ]  [ ▶ ]  [ ❚❚ ]  [ → ]                              |
|                               H1  Hair by Lydia                                      |
|                            Short intro line (paragraph)                              |
+--------------------------------------------------------------------------------------+
|                                  H2  About Lydia                                     |
|                                                                                      |
|                +-----------+       H3  What Lydia does                                |
|                |   Photo   |       About text (paragraph)                             |
|                |  (Lydia)  |                                                          |
|                +-----------+                                                         |
|                    Not sure what to book?  [ Ask Lydia → ]                           |
|                      [ Gallery ]  [ Services ]  [ Enquire ]                          |
+--------------------------------------------------------------------------------------+
|                                H2  What clients say                                  |
|                                Review text (paragraph)                               |
|                                Reviewer name                                         |
|                         [ ← ]   [ ❚❚ ]   1 of 5   [ → ]                              |
|                                Read all reviews →                                    |
+--------------------------------------------------------------------------------------+
| • Home →                • Gallery →                                        (IG)      |
| • Services + Prices →   • Reviews →                                        (FB)      |
| • Enquire →             • FAQ →                                            (WA)      |
|                                                                                      |
| Hair by Lydia                                                                        |
| Rights etc.                                                                          |
+--------------------------------------------------------------------------------------+
```

## Services and Prices

**Goal:** Let visitors see what Lydia offers and what it costs, then enquire.
**Source:** [servicehandnote.jpg](./screenshots/handnote/servicehandnote.jpg)
**Status:** Sketched

### Hand note
![Services hand note](./screenshots/handnote/servicehandnote.jpg)

### Wireframe - Services & Pricing Mobile (US06)

```text
+------------------------------------------------+
| ✱ Hair By Lydia →          [ Enquire ] [ Menu ]|
+------------------------------------------------+
|            H1  Services + Prices               |
|        Intro (paragraph)                       |
|        Covers Banbury + surrounding villages   |
|                                                |
|   H2  Service A            From £xx            |
|   Short description (paragraph)                |
|   H2  Service B            From £xx            |
|   Short description (paragraph)                |
|   H2  Service C            From £xx            |
|   Short description (paragraph)                |
|                                                |
|   Note: extra travel charges may apply,        |
|   discussed before confirmation                |
+------------------------------------------------+
|             H2  What clients say               |
|           Review text (paragraph)              |
|           Reviewer name                        |
|   [ ← ]    [ ❚❚ ]   1 of 5    [ → ]            |
|          Read all reviews →                    |
+------------------------------------------------+
| • Home →               • Gallery →     (IG)    |
| • Services + Prices →  • Reviews →     (FB)    |
| • Enquire →            • FAQ →         (WA)    |
|                                                |
| Hair by Lydia                                  |
| Rights etc.                                    |
+------------------------------------------------+
```

### Wireframe - Services & Pricing Desktop (US06)
```text
+--------------------------------------------------------------------------------------+
| ✱ Hair By Lydia →   Home →  Services and Prices →  Gallery →  Reviews →  FAQ → [Enquire] |
+--------------------------------------------------------------------------------------+
|                             H1  Services + Prices                                    |
|                             Intro (paragraph)                                        |
|                      Covers Banbury + surrounding villages                           |
|                                                                                      |
|                  H2  Service A ........ From £xx                                     |
|                  Short description (paragraph)                                       |
|                  H2  Service B ........ From £xx                                     |
|                  Short description (paragraph)                                       |
|                  H2  Service C ........ From £xx                                     |
|                  Short description (paragraph)                                       |
|                                                                                      |
|          Note: extra travel charges may apply, discussed before confirmation         |
+--------------------------------------------------------------------------------------+
|                                H2  What clients say                                  |
|                                Review text (paragraph)                               |
|                                Reviewer name                                         |
|                         [ ← ]   [ ❚❚ ]   1 of 5   [ → ]                              |
|                                Read all reviews →                                    |
+--------------------------------------------------------------------------------------+
| • Home →                • Gallery →                                        (IG)      |
| • Services + Prices →   • Reviews →                                        (FB)      |
| • Enquire →             • FAQ →                                            (WA)      |
|                                                                                      |
| Hair by Lydia                                                                        |
| Rights etc.                                                                          |
+--------------------------------------------------------------------------------------+
```

## Gallery

**Goal:** Show visitors Lydia's real work, including before-and-after results, so they can judge her style before enquiring.
**Source:** [galleryhandnote.jpg](./screenshots/handnote/galleryhandnote.jpg)
**Status:** Sketched

### Hand note
![Gallery hand note](./screenshots/handnote/galleryhandnote.jpg)

### Wireframe - Gallery Mobile (US04)

```text
+------------------------------------------------+
| ✱ Hair By Lydia →          [ Enquire ] [ Menu ]|
+------------------------------------------------+
|                 H1  Gallery                    |
|              Intro (paragraph)                 |
|                                                |
|     +-------------+   +-------------+          |
|     | [ image ]   |   | [ image ]   |          |
|     | (alt text)  |   | (alt text)  |          |
|     | Caption 1   |   | Caption 2   |          |
|     +-------------+   +-------------+          |
|     +-------------+   +-------------+          |
|     | [ before |  |   | [ image ]   |          |
|     |   after ]   |   | (alt text)  |          |
|     | Caption 3   |   | Caption 4   |          |
|     | (Before/    |   |             |          |
|     |  After)     |   |             |          |
|     +-------------+   +-------------+          |
|                  [ More ]                      |
+------------------------------------------------+
|             H2  What clients say               |
|           Review text (paragraph)              |
|           Reviewer name                        |
|   [ ← ]    [ ❚❚ ]   1 of 5    [ → ]            |
|          Read all reviews →                    |
+------------------------------------------------+
| • Home →               • Gallery →     (IG)    |
| • Services + Prices →  • Reviews →     (FB)    |
| • Enquire →            • FAQ →         (WA)    |
|                                                |
| Hair by Lydia                                  |
| Rights etc.                                    |
+------------------------------------------------+
```

### Wireframe - Gallery Desktop (US04)

```text
+--------------------------------------------------------------------------------------+
| ✱ Hair By Lydia →   Home →  Services and Prices →  Gallery →  Reviews →  FAQ → [Enquire] |
+--------------------------------------------------------------------------------------+
|                                   H1  Gallery                                        |
|                               Intro (paragraph)                                      |
|                                                                                      |
|         +-------------+   +-------------+   +----------------+                         |
|         | [ image ]   |   | [ image ]   |   | [ before|after]|                         |
|         | (alt text)  |   | (alt text)  |   | (alt text)     |                         |
|         | Caption 1   |   | Caption 2   |   | Caption 3      |                         |
|         |             |   |             |   | (Before/After) |                         |
|         +-------------+   +-------------+   +----------------+                         |
|         (more rows of cards: same layout)                                            |
|                                 [ More ]                                             |
+--------------------------------------------------------------------------------------+
|                                H2  What clients say                                  |
|                                Review text (paragraph)                               |
|                                Reviewer name                                         |
|                         [ ← ]   [ ❚❚ ]   1 of 5   [ → ]                              |
|                                Read all reviews →                                    |
+--------------------------------------------------------------------------------------+
| • Home →                • Gallery →                                        (IG)      |
| • Services + Prices →   • Reviews →                                        (FB)      |
| • Enquire →             • FAQ →                                            (WA)      |
|                                                                                      |
| Hair by Lydia                                                                        |
| Rights etc.                                                                          |
+--------------------------------------------------------------------------------------+
```

## Reviews

**Goal:** Let visitors read genuine client reviews so they can trust Lydia before they enquire.
**Source:** [reviewhandnote.jpg](./screenshots/handnote/reviewhandnote.jpg)
**Status:** Sketched

### Hand note
![Reviews hand note](./screenshots/handnote/reviewhandnote.jpg)

### Wireframe - Reviews Mobile (US03)

```text
+------------------------------------------------+
| ✱ Hair By Lydia →          [ Enquire ] [ Menu ]|
+------------------------------------------------+
|                H1  Reviews                     |
|           Intro message (paragraph)            |
|                                                |
|   +----------------+   +----------------+      |
|   | ✱ Reviewer A   |   | ✱ Reviewer B   |     |
|   | Review text    |   | Review text    |      |
|   +----------------+   +----------------+      |
|   +----------------+   +----------------+      |
|   | ✱ Reviewer C   |   | ✱ Reviewer D   |     |
|   | Review text    |   | Review text    |      |
|   +----------------+   +----------------+      |
|   +----------------+                           |
|   | ✱ Reviewer E   |                           |
|   | Review text    |                           |
|   +----------------+                           |
|        (5 Lydia-approved reviews)              |
+------------------------------------------------+
| • Home →               • Gallery →     (IG)    |
| • Services + Prices →  • Reviews →     (FB)    |
| • Enquire →            • FAQ →         (WA)    |
|                                                |
| Hair by Lydia                                  |
| Rights etc.                                    |
+------------------------------------------------+
```

### Wireframe - Reviews Desktop (US03)

```text
+--------------------------------------------------------------------------------------+
| ✱ Hair By Lydia →   Home →  Services and Prices →  Gallery →  Reviews →  FAQ → [Enquire] |
+--------------------------------------------------------------------------------------+
|                                  H1  Reviews                                         |
|                            Intro message (paragraph)                                 |
|                                                                                      |
|          +--------------+  +--------------+  +--------------+                        |
|          | ✱ Reviewer A |  | ✱ Reviewer B |  | ✱ Reviewer C |                      |
|          | Review text  |  | Review text  |  | Review text  |                        |
|          +--------------+  +--------------+  +--------------+                        |
|                +--------------+  +--------------+                                    |
|                | ✱ Reviewer D |  | ✱ Reviewer E |                                   |
|                | Review text  |  | Review text  |                                    |
|                +--------------+  +--------------+                                    |
|                        (5 Lydia-approved reviews)                                    |
+--------------------------------------------------------------------------------------+
| • Home →                • Gallery →                                        (IG)      |
| • Services + Prices →   • Reviews →                                        (FB)      |
| • Enquire →             • FAQ →                                            (WA)      |
|                                                                                      |
| Hair by Lydia                                                                        |
| Rights etc.                                                                          |
+--------------------------------------------------------------------------------------+

```

## Enquiry

**Goal:** Let visitors ask Lydia a question or request advice, knowing an enquiry is not a confirmed booking.
**Source:** [enquireformhandnote.jpg](./screenshots/handnote/enquireformhandnote.jpg)
**Status:** Sketched

### Hand note
![Enquiry form hand note](./screenshots/handnote/enquireformhandnote.jpg)

### Wireframe - Enquiry Mobile (US05)

```text
+------------------------------------------------+
| ✱ Hair By Lydia →          [ Enquire ] [ Menu ]|
+------------------------------------------------+
|            H1  Enquire / Contact               |
|        Text about the form (paragraph)         |
+------------------------------------------------+
|              H2  Enquire form                  |
|            Name (required)                     |
|           [____________________]               |
|            Phone (required)                    |
|           [____________________]               |
|            Email (optional)                    |
|           [____________________]               |
|            Full address (required)             |
|           [____________________]               |
|    How did you hear about Lydia? (optional)    |
|           [ Select one       ▾ ]               |
|    What would you like? Tell Lydia about       |
|    your enquiry (required)                     |
|           +--------------------+               |
|           |                    |               |
|           +--------------------+               |
|              [ Send enquiry ]                  |
|                                                |
|              H3  Social media                  |
|        (IG)  (FB)  (WA)  Phone →               |
+------------------------------------------------+
|             H2  What clients say               |
|           Review text (paragraph)              |
|           Reviewer name                        |
|   [ ← ]    [ ❚❚ ]   1 of 5    [ → ]            |
|          Read all reviews →                    |
+------------------------------------------------+
| • Home →               • Gallery →     (IG)    |
| • Services + Prices →  • Reviews →     (FB)    |
| • Enquire →            • FAQ →         (WA)    |
|                                                |
| Hair by Lydia                                  |
| Rights etc.                                    |
+------------------------------------------------+
```

### Wireframe - Enquiry Desktop (US05)

```text
+--------------------------------------------------------------------------------------+
| ✱ Hair By Lydia →   Home →  Services and Prices →  Gallery →  Reviews →  FAQ → [Enquire] |
+--------------------------------------------------------------------------------------+
|                              H1  Enquire / Contact                                   |
|                         Text about the form (paragraph)                              |
+--------------------------------------------------------------------------------------+
|                                H2  Enquire form                                      |
|                              Name (required)                                         |
|                          [________________________]                                  |
|                              Phone (required)                                        |
|                          [________________________]                                  |
|                              Email (optional)                                        |
|                          [________________________]                                  |
|                         Full address (required)                                      |
|                          [________________________]                                  |
|                  How did you hear about Lydia? (optional)                            |
|                          [ Select one          ▾ ]                                   |
|            What would you like? Tell Lydia about your enquiry (required)             |
|                          +------------------------+                                  |
|                          |                        |                                  |
|                          +------------------------+                                  |
|                              [ Send enquiry ]                                        |
|                                                                                      |
|                              H3  Social media                                        |
|                         (IG)   (FB)   (WA)   Phone →                                 |
+--------------------------------------------------------------------------------------+
|                                H2  What clients say                                  |
|                                Review text (paragraph)                               |
|                                Reviewer name                                         |
|                         [ ← ]   [ ❚❚ ]   1 of 5   [ → ]                              |
|                                Read all reviews →                                    |
+--------------------------------------------------------------------------------------+
| • Home →                • Gallery →                                        (IG)      |
| • Services + Prices →   • Reviews →                                        (FB)      |
| • Enquire →             • FAQ →                                            (WA)      |
|                                                                                      |
| Hair by Lydia                                                                        |
| Rights etc.                                                                          |
+--------------------------------------------------------------------------------------+
```

## FAQ

**Goal:** Give visitors clear answers on cancellations and deposits before they enquire, without inventing any policy Lydia hasn't confirmed.
**Source:** No hand note yet. See US07 in [user-stories.md](./user-stories.md).
**Status:** Not sketched

### Wireframe - FAQ Mobile (US07)

```text
+------------------------------------------------+
| ✱ Hair By Lydia →          [ Enquire ] [ Menu ]|
+------------------------------------------------+
|                 H1  FAQ                        |
|           Intro message (paragraph)            |
|                                                |
|     • Question                                 |
|       Answer (always visible)                  |
|     • Question                                 |
|       Answer (always visible)                  |
|     • Question                                 |
|       Answer (always visible)                  |
+------------------------------------------------+
|             H2  What clients say               |
|           Review text (paragraph)              |
|           Reviewer name                        |
|   [ ← ]    [ ❚❚ ]   1 of 5    [ → ]            |
|          Read all reviews →                    |
+------------------------------------------------+
| • Home →               • Gallery →     (IG)    |
| • Services + Prices →  • Reviews →     (FB)    |
| • Enquire →            • FAQ →         (WA)    |
|                                                |
| Hair by Lydia                                  |
| Rights etc.                                    |
+------------------------------------------------+

```

### Wireframe - FAQ Desktop (US07)

```text
+--------------------------------------------------------------------------------------+
| ✱ Hair By Lydia →   Home →  Services and Prices →  Gallery →  Reviews →  FAQ → [Enquire] |
+--------------------------------------------------------------------------------------+
|                                    H1  FAQ                                           |
|                            Intro message (paragraph)                                 |
|                                                                                      |
|                       • Question                                                     |
|                         Answer (always visible)                                      |
|                       • Question                                                     |
|                         Answer (always visible)                                      |
|                       • Question                                                     |
|                         Answer (always visible)                                      |
+--------------------------------------------------------------------------------------+
|                                H2  What clients say                                  |
|                                Review text (paragraph)                               |
|                                Reviewer name                                         |
|                         [ ← ]   [ ❚❚ ]   1 of 5   [ → ]                              |
|                                Read all reviews →                                    |
+--------------------------------------------------------------------------------------+
| • Home →                • Gallery →                                        (IG)      |
| • Services + Prices →   • Reviews →                                        (FB)      |
| • Enquire →             • FAQ →                                            (WA)      |
|                                                                                      |
| Hair by Lydia                                                                        |
| Rights etc.                                                                          |
+--------------------------------------------------------------------------------------+
```