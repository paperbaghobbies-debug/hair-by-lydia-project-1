# Feature Research and Decisions

**Status:** Working research and decision log for Sprint 0. Client input, student proposals and items still needing confirmation are labelled below.

## Source key

| Tag | Meaning |
|---|---|
| **[Q]** | Information or feedback provided by Lydia |
| **[P]** | Student proposal, interpretation or assumption |
| **[C]** | To confirm or verify before treating as final |

## 1. Hosting and running costs

**Requirement:** Keep hosting inexpensive, secure and low-maintenance (Q23, Q26).

**Research:** I compared GitHub Pages with Cloudflare's free options. The research notes flag GitHub Pages' terms for commercial use and identify Cloudflare Pages as a possible fit. Sources: [Cloudflare plans](https://www.cloudflare.com/plans/#application-services), [Cloudflare Pages pricing](https://www.cloudflare.com/plans/free/), [GitHub Pages limits](https://docs.github.com/en/pages/getting-started-with-github-pages/github-pages-limits), and [Cloudflare Pages vs Workers](https://flaviocopes.com/cloudflare-pages-vs-workers/). Screenshot evidence: [Cloudflare limits](screenshots/cloudflare-limits-research-1.png), [Cloudflare plan price](screenshots/cloudflare-price-research.png), [GitHub Pages limits](screenshots/github-limits-research.png), and [GitHub Pages terms](screenshots/github-pages-terms.png).

**Proposal:** Use Cloudflare Pages on the free plan if it supports the final features and meets the site's needs. **[P]**

**To confirm:** Check current limits, commercial-use terms, compatibility with the planned features and any costs before confirming the host. **[C]**

## 2. Custom domain

**Requirement:** Lydia would like a custom domain at a low cost (Q23).

**Research:** Cloudflare's domain-pricing information was reviewed: [How much does a domain name cost?](https://www.cloudflare.com/learning/dns/how-much-does-a-domain-name-cost/). Screenshot evidence: [Cloudflare pricing research](screenshots/cloudflare-price-research.png).

**Proposal:** Connect the site to a custom domain through Cloudflare if the final hosting choice supports it. A domain name may still have a registration cost; compare the total price before purchase. **[P]**

**To confirm:** Confirm the preferred domain name, registration cost and renewal cost with Lydia. **[C]**

## 3. Enquiry form delivery

**Requirement:** Send enquiries to Lydia with minimal cost and maintenance (Q11, Q17).

**Research:** I compared Cloudflare Email Service with FormSubmit. The research notes say Cloudflare Email Routing is included on Workers Free and describe sending to a verified destination; this still needs to be tested with the planned Pages Function. The notes also say FormSubmit allows unlimited forms and submissions at no cost and keeps submissions in an archive for 30 days. Check the providers' current documentation and terms before relying on these details: [FormSubmit](https://formsubmit.co/). Screenshot evidence: [Cloudflare email research 1](screenshots/cloudflare-email-research-1.png), [Cloudflare email research 2](screenshots/cloudflare-email-research-2.png), and [Cloudflare email research 3](screenshots/cloudflare-email-research-3.png).

**Proposal:** Use FormSubmit to email enquiries to Lydia, who can reply to clients from her usual email account. Keep spam protection enabled. **[P]**

**To confirm:** Test the full enquiry and reply workflow, verify delivery, and check FormSubmit's privacy information, terms, archive behaviour and spam protection before using it on the live site. **[C]**

## 4. Photo uploads with enquiries

**Requirement:** Lydia mentioned photo uploads as an optional enquiry feature (Q17). **[Q]**

**Proposal:** Keep photo uploads off the initial form. Ask clients to send photos by WhatsApp or email after Lydia has replied, to keep the form simple and avoid collecting images at first contact. **[P]**

**To confirm:** Check that Lydia is happy with this approach. **[C]**

## 5. Portfolio gallery and Instagram

**Requirement:** Lydia would like her existing Instagram gallery to inform the site's portfolio presentation (Q13, Q21, Q24). **[Q]**

**Research:** I reviewed the [Instagram API with Facebook Login](https://developers.facebook.com/documentation/instagram-platform/instagram-api-with-facebook-login), Meta's [content and intellectual-property policy](https://www.meta.com/en-gb/help/policies/2202628709913826/), and a [Stack Overflow discussion of displaying an Instagram gallery](https://stackoverflow.com/questions/12478772/how-do-i-use-instagrams-api-to-display-a-gallery-of-my-own-photos). The API approach has not yet been tested; research alone does not establish that it will work for this site or account.

**Proposal:** Investigate an Instagram API-fed gallery, with a hand-built gallery from Lydia's original images as a fallback if the API approach is unsuitable. **[P]**

**To confirm:** Test feasibility and maintenance needs, verify current API access and terms, and confirm image permissions and the fallback content with Lydia. **[C]**

## 6. Updating prices and other content

**Requirement:** Lydia would prefer a no-code way to make occasional updates. Updates are infrequent, so developer assistance was also considered.

**Research:** I considered [Cloudflare Workers KV](https://www.cloudflare.com/products/kv/) and the [Cloudflare community discussion about editing a website](https://community.cloudflare.com/t/edit-code-of-website-with-cloudflare/478014). Lydia said that maintaining a KV update system would be outside her skills. **[Q]** Screenshot evidence: [Cloudflare Workers limits research](screenshots/cloudflare-worker-limits-research-1.png).

**Proposal:** Do not build a self-service price-update feature for now. If Lydia requests a price change, update the prices in the site's HTML. **[P]**

## 7. Reviews and review carousel

**Requirement:** Present reviews selected by Lydia in a prominent and readable way. **[Q]**

**Research:** I reviewed [accessible carousel guidance](https://www.a11y-collective.com/blog/accessible-carousel/), a [reviews-carousel example](https://github.com/antonADev/reviews-carousel), and a [carousel implementation video](https://www.youtube.com/watch?v=nbNBe2bAw8c).

**Proposal:** Build a custom HTML, CSS and JavaScript carousel with manual previous/next controls. Keep the reviews readable without JavaScript, provide text alternatives for star ratings, and reuse the reviews as cards on a dedicated Reviews page. Do not use auto-rotation or Google Reviews integration. **[P]**

**To confirm:** Ask Lydia which reviews she wants to feature and confirm permission to publish them. **[C]**

## 8. Header behaviour

**Requirement:** Lydia liked the transparent, sticky header behaviour on a competitor site and wanted to explore whether a similar effect could suit her branding. **[Q]**

**Research:** I reviewed examples and guidance on [transparent scrolling headers](https://uicookies.com/snippets/transparent-scroll-header/), [scroll-linked header effects](https://uicookies.com/snippets/scroll-linked-header-effects/), [sticky header changes](https://vinish.dev/sticky-header-changes-on-scroll), [header design](https://wpdean.com/css-header/), [mobile and SEO considerations](https://www.j-a-b.net/how-to-design-a-sticky-header-that-does-not-hurt-mobile-ux-or-seo/), and [CSS sticky positioning](https://sizzy.co/blog/css-position-sticky). Screenshot evidence: [header behaviour research](screenshots/matthewgrant-header-research.png).

**Dated client note — 28/10/2026:** Lydia agreed to drop the transparent header. Her logo would not blend into a transparent navigation bar as it did on the reference site, so the agreed direction is a taupe header fixed from the top of the page. **[Q]**

**Implementation proposal:** Use a fixed taupe header from page load. **[P]** Check its behaviour on small screens and ensure it does not obscure page content. **[C]**

## 9. Fonts

**Requirement:** Lydia wants to keep Noto Serif Display Extra Condensed for “Hair by Lydia” on the main branding image and Luxurious Script for other branding. **[Q]**

**Research:** I checked the [Noto Serif Display specimen](https://fonts.google.com/specimen/Noto+Serif+Display) and its [SIL Open Font Licence](https://github.com/google/fonts/blob/main/ofl/notoserifdisplay/OFL.txt), and the [Luxurious Script specimen](https://fonts.google.com/specimen/Luxurious+Script) and its [SIL Open Font Licence](https://github.com/google/fonts/blob/main/ofl/luxuriousscript/OFL.txt).

**Proposal:** Use Lydia's selected fonts for the branding uses she specified. Choose a readable body font and present it to Lydia for review. **[P]**

**To confirm:** Review the body-font choice with Lydia. **[C]**

## 10. Image quality and loading

**Requirement:** Images should load reliably and have sufficient resolution to present Lydia's work well. **[Q]**

**Research:** I reviewed guidance on [lazy loading](https://www.debugbear.com/blog/lazy-loading-performance), [lazy-load performance](https://pagespeed.one/en/know-how/lazyload), [responsive images](https://developer.mozilla.org/en-US/docs/Web/HTML/Guides/Responsive_images), and [responsive images with `srcset`](https://docs.imgix.com/en-US/getting-started/tutorials/responsive-design/responsive-images-with-srcset).

**Proposal:** Use the Instagram API gallery if testing supports it, with a hand-built gallery as a fallback. Use responsive image techniques where appropriate and native lazy loading for below-the-fold images. **[P]**

**To confirm:** Test the chosen image source and image quality in the implemented site. **[C]**

## 11. Colour palette and contrast

**Requirement:** Keep Lydia's warm beige, cream and brown palette. **[Q]**

**Research:** I sampled the logo background as taupe `#7F7367` and checked combinations using the [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/) and [WCAG 2.2 contrast guidance](https://www.w3.org/WAI/WCAG22/Understanding/contrast-minimum.html). I also reviewed [WCAG 2.2 non-text contrast guidance](https://www.w3.org/WAI/WCAG22/Understanding/non-text-contrast.html).

| Foreground | Background | Contrast | Result recorded in research |
|---|---|---:|---|
| White `#FFFFFF` | Taupe `#7F7367` | 4.61:1 | WCAG AA for normal text |
| Dark brown `#342B24` | Cream `#FAF3EB` | 12.58:1 | WCAG AAA for normal text |
| Dark brown `#342B24` | Muted gold `#C6A15B` | 5.70:1 | WCAG AA for normal text |

**Proposal:** Use taupe for the navigation bar with white text, cream/off-white for the main background, dark brown for body text, and muted gold with dark-brown text for calls to action. **[P]**

**To confirm:** Check final rendered combinations, including hover, active and keyboard-focus states, and choose focus indicators that contrast with each surface. **[C]**

**Evidence:** [Navigation contrast](screenshots/contrast-nav-white-on-taupe.png), [body-text contrast](screenshots/contrast-body-dark-brown-on-cream.png), and [CTA contrast](screenshots/contrast-cta-dark-brown-on-gold.png).

## 12. Responsive layout and rendering

**Research:** I drew on my freeCodeCamp Responsive Web Design certificate and reviewed responsive-layout guidance from [MDN](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/CSS_layout/Responsive_Design), [Chrome DevTools device mode](https://developer.chrome.com/docs/devtools/device-mode/), and information about [HTML templates](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/template), [client-side rendering and SEO](https://developers.google.com/search/docs/crawling-indexing/javascript/javascript-seo-basics), and [rendering approaches](https://developers.google.com/solutions/content-driven/hosting/rendering). I also considered [client-side template trade-offs](https://stackoverflow.com/questions/16255859/client-side-templates-in-script-tags-advantages-disadvantages) and [template-engine trade-offs](https://hackernoon.com/pros-and-cons-of-popular-javascript-templating-engines).

**Proposal:** Use a mobile-first layout with flexible CSS and media queries, using Flexbox where suitable. Keep the main content in HTML rather than generating the whole site from JavaScript templates; use JavaScript only where needed for interactive or dynamic features. Test at different screen sizes. **[P]**

**To confirm:** Device emulation is useful for regular checks, but test on a real phone if one is available. Consider search visibility separately under item 14. **[C]**

## 13. “How did you hear about Lydia?” field

**Requirement:** Lydia would like to know how visitors heard about her. **[Q]**

**Proposal:** Add an optional enquiry-form dropdown with: word of mouth, Google/search, Instagram, Facebook, other, and prefer not to say. Include the selected answer in the enquiry email; do not add backend tracking. **[P]**

**To confirm:** Check the wording and options with Lydia and test that the response is included in the enquiry email. **[C]**

## 14. Search visibility and service area

**Requirement:** Lydia wants more potential clients to find the business online and enquire. The research notes say she does not currently use Google Business and describes her as a mobile hairdresser serving Banbury and surrounding areas. **[Q]**

**Research:** I reviewed Google's [SEO starter guide](https://developers.google.com/search/docs/fundamentals/seo-starter-guide), [JavaScript SEO guidance](https://developers.google.com/search/docs/crawling-indexing/javascript/javascript-seo-basics), guidance on [title links](https://developers.google.com/search/docs/appearance/title-link) and [snippets](https://developers.google.com/search/docs/appearance/snippet), and information about [Google Business Profile](https://support.google.com/business/answer/7091) and [eligibility](https://support.google.com/business/answer/3038177). Hair-salon keyword articles were used for phrase ideas, not as evidence of local search volume: [Seopital](https://www.seopital.co/blog/the-best-hair-salon-seo-keywords), [MarketKeep](https://marketkeep.com/seo-keywords-for-hair-salons/), [Ron Kot](https://www.ronkot.com/best-seo-keywords-for-hair-salons/), and [Digitally Top](https://digitallytop.com/digital-marketing/seo-for-hair-salons/).

**Proposal:** Use a multi-page site with important content in the HTML, clear page titles and descriptions, headings and crawlable links. Describe Lydia's services and Banbury service area naturally, without promising rankings or a fixed travel radius. Do not include Google Business Profile in the current plan. **[P]**

**To confirm:** Confirm travel availability and the service-area wording with Lydia. A multi-page site does not guarantee rankings, and no search-volume data has been established. **[C]**

## Evidence

- [Original feature research rough notes](../features-research-rough-notes.txt) — preserved as the source for this document, including the dated account of Lydia's header decision.
- Research screenshots are linked beside the relevant findings above.
