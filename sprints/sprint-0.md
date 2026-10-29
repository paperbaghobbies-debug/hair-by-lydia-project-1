# Sprint 0: Hair by Lydia

**Status:** This plan stays a draft until the **[C]** items are confirmed. Nothing is marked Done unless evidence exists and is linked.

## Source key

| Tag | Meaning |
|---|---|
| **[Q]** | Derived from the client questionnaire |
| **[P]** | Student proposal or assumption |
| **[C]** | To confirm (with Lydia, tutor or assessment criteria) |

---

## 1. Goal

By the end of Sprint 0, I will have a client-reviewed brief for Hair by Lydia, made up of researched feature decisions, reviewed user stories and rough wireframes, ready to start Sprint 1. **[P: tightened from original goal sentence, to confirm]**

"Client-reviewed" is used because it matches what the evidence can show (Lydia's recorded feedback on the brief). It becomes "client-confirmed" only if a sign-off message exists.

Evidence for each part:

| Part of goal | Evidence |
|---|---|
| Client-reviewed brief | Lydia's recorded feedback on the brief, plus a sign-off message if given. None yet. Link when the file exists |
| Researched feature decisions | Research and decision log, and competitor comparison. None yet. Link when the file exists |
| Reviewed user stories | User stories v2 are not yet present; v3 once finalised, plus Lydia's feedback. None yet. Link when the file exists |
| Rough wireframes | Wireframe files for key pages and widths. None yet. Link when the file exists |

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
| 3 | Research features and options | 2 | Research and decision log | Options compared for form delivery, photo upload, review layout, Instagram content, update method and hosting/costs; each has a recommendation and cited source; time-boxed | Each decision has options, a source and a recommendation | [`docs/feature-research.md`](../docs/feature-research.md), [`features-research-rough-notes.txt`](../features-research-rough-notes.txt) (original notes), [`docs/ai_log.md`](../docs/ai_log.md) (Entry 6) | Not started |
| 4 | Get Lydia's feedback | 3 | Feedback record | Follow-up questions sent covering all open questions from cards 1–3; responses (or chasers) recorded with dates | Every open item shows an answer or a stated assumption | None yet. Link when the file exists | Not started |
| 5 | Finalise user stories | 4 | User stories v3 | Stories updated for Lydia's answers; priorities confirmed; criteria testable and tagged | Each story traces to a questionnaire answer or feedback | None yet. Link when the file exists | Not started |
| 6 | Wireframe key pages | 5 | Rough wireframes (mobile and desktop) | Home, gallery, services and prices, enquiry form and FAQ covered; each maps to named stories | Wireframe checked against story list | None yet. Link when the file exists | Not started |
| 7 | Compile the complete brief | 6 | Brief document | Scope, audience, content list, design direction, features, decisions and constraints in one place; Lydia has reviewed it | Lydia's review (and sign-off if given) recorded | None yet. Link when the file exists | Not started |

## 5. Definition of Done

A card moves to Done only when:

- [ ] Its single output exists and is saved in the repository
- [ ] Every acceptance criterion has been checked and the result noted
- [ ] Evidence links only to files that exist; if a file does not exist yet, state "None yet. Link when the file exists"
- [ ] Board card is moved to Done and linked to the evidence file
- [ ] Any AI use is recorded in the AI log
- [ ] Assumptions are tagged **[P]** and open questions **[C]**
- [ ] Spoken agreements with Lydia are recorded in a dated note the same day
- [ ] At sprint end, clear every **[C]** tag by confirming it or replacing it with a documented assumption; remove obsolete placeholders and fill in "Actual hours" at the end of each card
- [ ] Nothing is claimed that the evidence does not show

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

**[C: order to be confirmed]**

## 8. Timeline

### Dates

| Item | Date |
|---|---|
| Start | Tue 27 Oct 2026 **[P]** (planned) |
| Planned end | Wed 4 Nov 2026 **[P]** |

### Hours

| Card | Planned hours | Target date | Actual hours | Notes |
|---|---|---|---|---|
| 1. Summarise client needs | 3 | Tue 27 Oct **[P]** | | |
| 2. Competitor research | 3 | Wed 28 Oct **[P]** | | Three sites, same checklist |
| 3. Research features and options | 3 | Thu 29 Oct **[P]** | | Time-boxed; hosting options first |
| 4. Get Lydia's feedback | 3 | Fri 30 Oct **[P]** | | Questions sent by 29 Oct; includes time for Lydia to reply |
| 5. Finalise user stories | 4 | Mon 2 Nov **[P]** | | Depends on Lydia's answers |
| 6. Wireframe key pages | 5 | Tue 3 Nov **[P]** | | |
| 7. Compile the complete brief | 3 | Wed 4 Nov **[P]** | | Includes Lydia's review |
| **Total** | **26** | | | |

### Contingency

The approximately 5 h contingency (20% of 26 h) is covered by spare capacity within the 35 h available across the 7 planned workdays; it is not separately allocated to a card. If work finishes early, the spare time is not used to cut checks or evidence. **[P]**

Sat 31 Oct and Sun 1 Nov are rest days, not planned work or contingency capacity. **[P]**

### Change cut-off

30th October 2026 (Fri) **[P]**. This freezes new ideas before card 5 starts on 2 Nov; later ideas go to the Sprint 1 backlog and are recorded in the dated note. Answers to questions already asked are not new ideas.

The cut-off is after card 4 so feedback can still arrive while cards 5 and 6 are being prepared; input received by 30 Oct can be incorporated. **[P]**

### Check

The 4 Nov end date leaves about 7 weeks (51 days) before 25 Dec for Sprints 1-2; confirm this against the sprint estimates. **[C]**

## 9. Review

*Leave blank until the end of the sprint.*

| Item | Entry |
|---|---|
| Date | |
| Goal vs outcome | |

| Merit criterion | Evidence location |
|---|---|
| | |

## 10. Retrospective

*Leave blank until the end of the sprint.*

**What went well**

**What to change**