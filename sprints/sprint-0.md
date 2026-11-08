# Sprint 0: Hair by Lydia
**Current position:** Sprint 0 closed on 8 November 2026 after review. All Sprint 0 cards are recorded as done for this sprint; outstanding research, experiments and checks are carried forward to the relevant later sprints.

## Source key

| Tag | Meaning |
|---|---|
| **[Q]** | Derived from the client questionnaire |
| **[P]** | Student proposal or assumption |
| **[C]** | To confirm (with Lydia, tutor or assessment criteria) |

---

## 1. Goal

By the end of Sprint 0, I will have a client-reviewed brief for Hair by Lydia, made up of researched feature decisions, reviewed user stories and rough wireframes, ready to start Sprint 1.

I treat Lydia's positive email response as formal sign-off of the brief she reviewed on 6 November 2026. It does not automatically sign off later changes.

Evidence for each part:

| Part of goal | Evidence |
|---|---|
| Client needs | [Questionnaire](../docs/questionaire-hbl.md) and [requirements mapping](../docs/requirements-mapping.md): Q1–Q26 are mapped to needs, features and open questions. |
| Lydia's feedback | [Feedback record](../docs/lydia-feedback.md): responses and remaining decisions are recorded; further feedback can be sought during development. |
| Client-reviewed brief | [Website brief](../docs/brief.md) and [Lydia's review response](../docs/screenshots/lydia-brief-review.png), dated 6 November 2026. I treat her response as sign-off of the version she reviewed. |
| Researched feature decisions | [Feature research and decision log](../docs/feature-research.md) and [competitor comparison](../docs/competitor-research.md) exist. Some research checks and decisions remain open; see cards 2–3 below. |
| Reviewed user stories | [User stories](../docs/user-stories.md), linked to the [requirements mapping](../docs/requirements-mapping.md) and feedback. I reviewed the stories for Sprint 0 closure; remaining implementation and verification work is carried forward. |
| Design principles | [Design principles and accessibility](../docs/design-principles-accessibility.md): research-informed decisions and planned accessibility checks. |
| Rough wireframes | [Mobile and desktop wireframes](../docs/wire-frames.md), checked against the [user stories](../docs/user-stories.md); review and decision record in [AI log Entry 9](../docs/ai_log.md). |

## 2. Scope

Planning only, no code.

1. Understand the client's needs and the brief **[P]**
2. Research features and options (including competitor sites) **[P]**
3. Get Lydia's feedback on them **[P]**
4. Develop the user stories **[P]**
5. Plan the site's look and function, including rough wireframes **[P]**
6. End with a client-reviewed brief **[P]**

Governance and workflow: counted as already evidenced by the AI-rules card (Done on the board), not as new Sprint 0 work. **[C: confirm this decision]**

## 3. Out of scope

- Writing site code (HTML, CSS, JavaScript)
- Deployment, hosting setup and domain registration
- Final visual design and polished mock-ups
- Content creation beyond what the brief needs (for example, final About Me copy)
- Anything else deferred to Sprint 1 **[C]**

## 4. Work plan

One card, one clear output.

| # | Card title | Scope item | Output | Acceptance criteria | Planned check | Evidence location | Status |
|---|---|---|---|---|---|---|---|
| 0 | AI rules and workflow set up | Governance (pre-existing) | AI rules document | Rules written and saved in the repository; AI use recorded in the AI log | Board shows Done; rules file and AI log open and match | [`docs/hbl-ai-rules.md`](../docs/hbl-ai-rules.md), [`docs/ai_log.md`](../docs/ai_log.md) | Done (per board) |
| 1 | Summarise client needs from questionnaire | 1 | Requirements summary (one page) | Every Q1-Q26 answer mapped to a need, feature or constraint; gaps listed | Check each question number appears | [`docs/requirements-mapping.md`](../docs/requirements-mapping.md), [`docs/ai_log.md`](../docs/ai_log.md) (Entries 2 and 3) | Done (per board, issue #2) |
| 2 | Competitor research | 2 | Competitor comparison (three sites) | Three hairdresser websites reviewed against the same checklist (layout, gallery, prices, enquiry route, mobile, basic accessibility); includes any sites Lydia named in Q6 if she supplies them; features to adopt or avoid listed | Each site scored on the same checklist; takeaways link to stories or decisions | [`docs/competitor-research.md`](../docs/competitor-research.md), [`docs/lydia-competitor-rough-notes.txt`](../docs/lydia-competitor-rough-notes.txt), [`docs/ai_log.md`](../docs/ai_log.md) (Entry 5) | Done (per board, issue #3) |
| 3 | Research features and options | 2 | Research and decision log | Options compared for form delivery, photo upload, review layout, Instagram content, update method and hosting/costs; each has a recommendation and cited source; time-boxed | Each decision has options, a source and a recommendation | [`docs/feature-research.md`](../docs/feature-research.md), [`features-research-rough-notes.txt`](../notes/features-research-rough-notes.txt) (original notes), [`docs/ai_log.md`](../docs/ai_log.md) (Entry 6) | Done for Sprint 0 — research completed for this stage; further research and experiments are carried forward before features are added to the finished project. Card closed per my review. |
| 4 | Get Lydia's feedback | 3 | Feedback record | Follow-up questions sent covering all open questions from cards 1–3; responses (or chasers) recorded with dates | Every open item shows an answer or a stated assumption | [`docs/lydia-feedback.md`](../docs/lydia-feedback.md), [`docs/questionaire-hbl.md`](../docs/questionaire-hbl.md), [`docs/requirements-mapping.md`](../docs/requirements-mapping.md) | Done for Sprint 0 — feedback to date is complete; further feedback will be sought as needs arise. |
| 5 | Finalise user stories | 4 | User stories v3 | Stories updated for Lydia's answers; priorities confirmed; criteria testable and tagged | Each story traces to a questionnaire answer or feedback | [`docs/user-stories.md`](../docs/user-stories.md), [`docs/requirements-mapping.md`](../docs/requirements-mapping.md), [`docs/lydia-feedback.md`](../docs/lydia-feedback.md) | Done for Sprint 0 — I reviewed the stories and priorities; implementation and verification are carried forward. |
| 6 | Wireframe key pages | 5 | Rough wireframes (mobile and desktop) | Home, gallery, services and prices, enquiry form and FAQ covered; each maps to named stories | Wireframe checked against story list | [`docs/wire-frames.md`](../docs/wire-frames.md), [`docs/user-stories.md`](../docs/user-stories.md), [`docs/ai_log.md`](../docs/ai_log.md) (Entry 9) | Done; review and decisions recorded |
| 7 | Compile the complete brief | 6 | Brief document | Scope, audience, content list, design direction, features, decisions and constraints in one place; Lydia has reviewed it | Lydia's review (and sign-off if given) recorded | [`docs/brief.md`](../docs/brief.md), [Lydia's review response](../docs/screenshots/lydia-brief-review.png) | Done for Sprint 0 — brief complete; I treat Lydia's response as sign-off of the version she reviewed. |

Related GitHub issues [#5](https://github.com/paperbaghobbies-debug/hair-by-lydia-project-1/issues/5) (open questions) and [#8](https://github.com/paperbaghobbies-debug/hair-by-lydia-project-1/issues/8) (design principles) are closed. Issue [#11](https://github.com/paperbaghobbies-debug/hair-by-lydia-project-1/issues/11) covers the initial [README](../readme.md) and [testing record](../testing.md) templates; I confirmed its board card is Done, and both documents will continue to be updated across sprints. It was not a separate row in the original work plan. Issue #8's evidence section and checkboxes still need updating.

## 5. Definition of Done

The original planned checks were:

- [ ] Its single output exists and is saved in the repository
- [ ] Every acceptance criterion has been checked and the result noted
- [ ] Evidence links only to files that exist; if a file does not exist yet, state "None yet. Link when the file exists"
- [ ] Board card is moved to Done and linked to the evidence file
- [ ] Any AI use is recorded in the AI log
- [ ] Spoken agreements with Lydia are recorded in a dated note the same day
- [ ] At sprint end, record unresolved questions and their next action, remove obsolete placeholders, and fill in "Actual hours" at the end of each card. For future sprints, **[Q]**, **[P]** and **[C]** tags are optional; there is no requirement to add or clear them.
- [ ] Nothing is claimed that the evidence does not show

**Closure note:** I consider the planning cards complete for Sprint 0 and confirmed that the project-board cards are in Done. The unchecked boxes above preserve the original checks; they do not establish that each check was individually verified. Some issue records and actual hours still need alignment, and the same-day record of every spoken agreement has not been independently verified. Open feature decisions and experiments are carried forward in section 11. AI assistance is recorded in the [AI log](../docs/ai_log.md) and [appendix](../docs/appendix.md); I still need to confirm assessment requirements with my assessor.

The GitHub issue state is separate from the board column: at the closure-evidence review, issues [#10](https://github.com/paperbaghobbies-debug/hair-by-lydia-project-1/issues/10) and [#11](https://github.com/paperbaghobbies-debug/hair-by-lydia-project-1/issues/11) were still open. Issue [#6](https://github.com/paperbaghobbies-debug/hair-by-lydia-project-1/issues/6) was closed with an original acceptance checkbox unchecked; feedback is complete for this stage, with further questions carried forward. These issue records need updating to reflect the closure evidence.

## 6. Dependencies and risks

| Risk | If it happens |
|---|---|
| Lydia unavailable | Send one reminder after a few days; record the delay; proceed with clearly tagged assumptions and mark the brief "assumptions to confirm" **[P]** |
| Research grows without limit | Time-box each decision; stop at two or three realistic options and a recommendation **[P]** |
| Brief sign-off is delayed or partial | Record what was and wasn't agreed; carry unresolved items into Sprint 1 as listed risks **[P]** |
| Key decisions depend on hosting choice (forms, uploads, updates) | Decide hosting early in card 3, then base the other decisions on it **[P]** |
| Cards become vague ("do research") | Re-check each card has one concrete output before starting it **[P]** |

## 7. Order and WIP

**Maximum two active cards at once.**

1. Card 1: Summarise client needs
2. Card 2: Competitor research (can run alongside card 1)
3. Card 3: Research features and options (can run alongside card 2, but only starts once card 1 is done, so no more than two cards are active)
4. Card 4: Get Lydia's feedback (sent once cards 1 to 3 identify the questions)
5. Card 5: Finalise user stories
6. Card 6: Wireframe key pages
7. Card 7: Compile the complete brief


## 8. Timeline

### Dates

| Item | Date |
|---|---|
| Start | Tue 27 Oct 2026 **[P]** (planned) |
| Planned end | Wed 4 Nov 2026 **[P]** |
| Actual closure | Sun 8 Nov 2026, following my review |

### Actual milestones

These are recorded milestones, not necessarily the dates all work on each task took place.

| Date | Milestone | Evidence or basis |
|---|---|---|
| 27 October 2026 | Requirements mapping and competitor research issues closed | [#2](https://github.com/paperbaghobbies-debug/hair-by-lydia-project-1/issues/2) and [#3](https://github.com/paperbaghobbies-debug/hair-by-lydia-project-1/issues/3). |
| 29 October 2026 | Feature research, open questions and Lydia's feedback issues closed | [#4](https://github.com/paperbaghobbies-debug/hair-by-lydia-project-1/issues/4), [#5](https://github.com/paperbaghobbies-debug/hair-by-lydia-project-1/issues/5) and [#6](https://github.com/paperbaghobbies-debug/hair-by-lydia-project-1/issues/6). |
| 3 November 2026 | User-story issue closed | [#7](https://github.com/paperbaghobbies-debug/hair-by-lydia-project-1/issues/7). |
| 5 November 2026 | Design-principles and wireframe issues closed | [#8](https://github.com/paperbaghobbies-debug/hair-by-lydia-project-1/issues/8) and [#9](https://github.com/paperbaghobbies-debug/hair-by-lydia-project-1/issues/9). |
| 6 November 2026 | Lydia responded positively to the brief she reviewed | [Lydia's review response](../docs/screenshots/lydia-brief-review.png). |
| 8 November 2026 | Sprint 0 closed after review | My closure decision and the review in section 9. |

### Hours

| Card | Planned hours | Target date | Actual hours | Notes |
|---|---|---|---|---|
| 1. Summarise client needs | 3 | Tue 27 Oct **[P]** | Not recorded | |
| 2. Competitor research | 3 | Wed 28 Oct **[P]** | Unclear | Issue #3 says “27 Oct 23.11”; it is unclear whether this is a time of day or a duration. |
| 3. Research features and options | 3 | Thu 29 Oct **[P]** | 4 h | Issue #4; hosting and costs remain subject to later verification. |
| 4. Get Lydia's feedback | 3 | Fri 30 Oct **[P]** | 2 h | Issue #6; includes time for Lydia to reply. |
| 5. Finalise user stories | 4 | Mon 2 Nov **[P]** | 3 h | Issue #7. |
| 6. Wireframe key pages | 5 | Tue 3 Nov **[P]** | 4.5 (5 Nov) | Completed; evidence linked in card 6 |
| 7. Compile the complete brief | 3 | Wed 4 Nov **[P]** | 3 h | Issue #10. |
| **Total** | **26** | | **Incomplete** | Not all actual hours are recorded. |

Issue #5 separately records 1 hour for compiling open questions. Issue #8 does not record actual hours. These issues are not separate rows in the original estimate, so their times are not included in the planned total above.

### Contingency

The approximately 5 h contingency (20% of 26 h) is covered by spare capacity within the 35 h available across the 7 planned workdays; it is not separately allocated to a card. If work finishes early, the spare time is not used to cut checks or evidence. **[P]**

Sat 31 Oct and Sun 1 Nov are rest days, not planned work or contingency capacity. **[P]**

### Change cut-off

30th October 2026 (Fri) **[P]**. This freezes new ideas before card 5 starts on 2 Nov; later ideas go to the Sprint 1 backlog and are recorded in the dated note. Answers to questions already asked are not new ideas.

The cut-off is after card 4 so feedback can still arrive while cards 5 and 6 are being prepared; input received by 30 Oct can be incorporated. **[P]**

### Check

The original 4 Nov planned end date leaves about 7 weeks (51 days) before 25 Dec. Sprint 0 closed on 8 Nov; confirm the revised page-sprint schedule against available time and estimates. **[C]**

## 9. Review

| Item | Entry |
|---|---|
| Date | 8 November 2026 |
| Goal vs outcome | Sprint 0 planning is closed following my review of the brief, user stories and research. Lydia responded positively to the brief she reviewed, and I treat her response as sign-off of that version. Further research, experiments and outstanding checks are carried forward to relevant later sprints. I feel that we have reached the point where further theoretical research alone will not move the project forward. We now need practical testing and experiments to evaluate the approaches identified. |



## 10. Retrospective

### What went well

- Breaking the work into a step-by-step plan helped me organise the
  Sprint 0 planning work.
- Through research, I found that there are many industry-standard methods
  and techniques that can help me achieve what I want in this build. This
  gave me approaches to explore rather than having to work everything out
  from scratch.

### What I would change

- Dense research took longer than expected. I will try using a screen
  reader for external sources and allow enough time to review them.
- I want to work out a clearer framework for staying on task, so that
  research, planning and development remain focused on the sprint goal.
- I will keep closer oversight of AI suggestions and check them against
  my own decisions and the project evidence.

### Actions for the next sprint

- Use the sprint goal and card acceptance criteria to keep work focused.
- Review progress against the schedule and carry new ideas into the
  backlog rather than letting them interrupt the current task.
- Keep the plan simple and identify fallbacks where a feature or
  dependency may not work as expected.

## 11. Carry-forward backlog and later specification

These items are planned or awaiting client clarification; they are not Sprint 0 completion evidence. Do not treat implementation as complete until applicable criteria below have been checked and linked to actual evidence.

| Item | Traceability | Next check / evidence required | Status |
|---|---|---|---|
| Verify enquiry privacy and data handling | US05 | US05 includes a required full-address field. Before enabling submissions, verify the form provider, recipients/processors, access and protection, retention and deletion, and contact route. Make accurate privacy information accessible from the form, footer and FAQ. | Enquiry sprint; before live submissions |
| Confirm the consultation flow | US05; Q8 and Q10 in the [requirements mapping](../docs/requirements-mapping.md) | Confirm whether the form is the online consultation's starting point or whether Lydia follows up separately. Preserve the client-confirmed rule that she consults before manually confirming a service and appointment. | Enquiry sprint; open |
| Verify Instagram feasibility | US04; [feature research](../docs/feature-research.md) | Research and experiment with Instagram display before adding it; use the approved hand-built fallback if impractical. | Gallery sprint |
| Verify ongoing costs and content maintenance | Q23, Q24 and Q26; sections 1, 2 and 6 of [feature research](../docs/feature-research.md) | Before the build/launch decision, verify registration and renewal costs, hosting and form/service charges, and maintenance/update costs. Record Lydia's stated expectation to own and pay for the domain; confirm its exact format, availability and renewal arrangement, and agree how photos, prices and other content will be updated. Record verified one-off and recurring amounts and link evidence. | Relevant feature decisions and integration/deployment; before commitments |
| Maintain README and testing records | [README](../readme.md); [testing record](../testing.md); issue #11 | Update the initial templates throughout development with actual implementation, test results, fixes and deployment details. | Across later sprints |
| Implement and evidence AC 2.1–2.9 | Project specification | Build at least three pages or page areas and evidence the applicable HTML/CSS validation, images, links, responsive layout, semantic markup, content and navigation. | Planned — later phase |
| Evidence documentation and maintainability for AC 3.1–3.9 | Project specification | Document purpose, user value and deployment in the README; add story-linked screenshots; attribute and distinguish external code; evidence the required code and file organisation. | Planned — later phase |
| Test and deploy for AC 5.1–5.5 | Project specification | Design and document manual tests, verify the deployed site against the development version, remove commented-out code from the final version and check internal links. Link actual results and deployment evidence. | Planned — later phase |
| Evidence Merit M(v)–M(vii) | Project specification | Document the project rationale and user stories in the README; record tests, bugs, fixes and any unresolved bugs; document the development lifecycle in the README. | Planned — later phase |