# Sprint 1: Hair by Lydia

**Status:** Draft plan. Dates, available hours and outstanding decisions
still need to be confirmed. No work is marked Done without evidence.

## Source key

| Tag | Meaning |
|---|---|
| **[Q]** | Derived from Lydia's questionnaire or feedback |
| **[P]** | My proposal or design decision |
| **[C]** | To confirm |

---

## 1. Goal

By the end of Sprint 1, I aim to have built and tested the Hair by Lydia
homepage, including its shared layout, introduction, approved content and
planned interactive features. **[P]**

The homepage should help visitors understand Lydia's service and find
their next step. **[Q/P]**

| Part of goal | Planned evidence |
|---|---|
| Homepage implementation | Homepage files and screenshots; link when available |
| Client needs | [Website brief](../docs/brief.md) and [user stories](../docs/user-stories.md) |
| Design | [Mobile and desktop wireframes](../docs/wire-frames.md) |
| Testing and fixes | [Testing record](../testing.md); results and evidence to be added |
| Sprint review | Section 9 below, completed at sprint end |

## 2. Scope

1. Check homepage requirements and identify approved or missing content.
2. Build the homepage structure and shared layout.
3. Add homepage content and agreed interactive features.
4. Test the homepage and record results.
5. Fix and retest issues found.
6. Review the sprint and record a short retrospective.

Relevant stories include US01 and US08, plus the homepage or shared
elements of US02, US03 and US09. The homepage review carousel is in scope;
the separate Reviews page belongs to its own later sprint. **[P]**

## 3. Out of scope

- Building the remaining page content; each page will have its own later sprint.
- Completing the enquiry form and its submission service.
- Registering a domain or completing final deployment.
- Claiming the entire website has been tested.
- Other work agreed for later sprints. **[C]**

Shared layout decisions may support later pages, but this sprint's
deliverable is the homepage. Where navigation points to a page not yet
built, provide a lightweight placeholder with a clear "Coming soon" message
and working links; do not treat the page content as complete.

## 4. Work plan

One card, one clear output. Card numbers and estimates are proposals
until I review them.

| # | Card title | Output | Acceptance criteria | Planned check | Evidence location | Status |
|---|---|---|---|---|---|---|
| 1 | Prepare homepage content | Homepage content and asset checklist | Relevant stories and wireframes reviewed; approved content, missing items and permissions recorded | Compare the checklist with the brief and ask Lydia about missing approvals | Brief, stories and approval evidence; link checklist if created | Planned |
| 2 | Build homepage structure | Semantic homepage and shared layout | Page has an appropriate title, landmarks, headings, navigation and footer; structure follows the agreed homepage design | Inspect the page and compare it with the wireframe | Homepage files and screenshots; link when available | Planned |
| 3 | Add homepage content and features | Homepage introduction, approved content and interactions | Relevant homepage story criteria are addressed; slideshow and featured-review carousel provide their required controls; outstanding content is identified | Check content against stories and operate each control | Homepage files, content approvals and test record; link evidence when available | Planned |
| 4 | Test and improve homepage | Completed test and retest record | Planned homepage checks have actual results; failures are fixed and retested or explicitly recorded as unresolved | Run the checks in Section 5 and record environment, results and evidence | [Testing record](../testing.md); evidence to be added | Planned |
| 5 | Review Sprint 1 | Sprint review and retrospective | Goal and card outcomes compared; unfinished work and next actions recorded; retrospective completed | Complete Sections 9–11 using actual evidence | This plan and linked evidence | Planned |

Navigation links to later pages should resolve to their lightweight
placeholders. The enquiry placeholder must clearly explain that the form is
not ready and offer the approved alternative contact route. Placeholder
pages do not satisfy the acceptance criteria for those stories.

## 5. Definition of Done and planned checks

A card moves to Done only when:

- [ ] Its output exists and is saved in the repository.
- [ ] Its changes are committed on the card's branch, with the relevant commit or merge recorded as evidence.
- [ ] Its acceptance criteria have been checked and results recorded.
- [ ] Relevant test procedures, actual results and retests are recorded.
- [ ] Evidence links point to files that exist.
- [ ] Content and images have the necessary approval for their intended use.
- [ ] Any AI use is recorded in the AI log.
- [ ] The board card is updated and linked to its evidence.
- [ ] Unfinished work and next actions are recorded.
- [ ] Nothing is claimed that the evidence does not show.

### Planned homepage checks

| Check | Expected result | Actual result / evidence |
|---|---|---|
| Layout at 320, 768 and 1280 CSS pixels | Content and controls remain available without overlapping or unwanted horizontal scrolling | Not tested |
| Keyboard use and focus | Interactive controls can be reached and operated; focus is visible | Not tested |
| Hero and review carousels | Hero previous/next and pause/resume controls work; the featured reviews carousel advances and its pause, previous and next controls work | Not tested |
| Images | Informative images have meaningful alternatives; decorative images have empty alternatives | Not tested |
| Contrast | Text and meaningful control boundaries meet the relevant WCAG AA thresholds in the rendered page | Not tested |
| Structure | Landmarks and headings give the page a clear structure | Not tested |
| Links | Links lead to their intended available destinations | Not tested |
| Content | Published copy and images have the necessary approval | Not checked |

Record the browser, version, device or emulator, viewport, steps and actual
result in [testing.md](../testing.md). Add fixes and retest results where
needed. Other devices or browsers should not be claimed as tested unless
they were actually checked.

## 6. Dependencies and risks

| Risk or dependency | Response |
|---|---|
| Approved hero or About images are delayed | Ask Lydia early; record what is missing and do not publish unapproved images. |
| Other pages do not yet exist | Decide and document how navigation should work during this sprint; test the agreed behaviour. |
| Testing is left too late | Reserve time for checks and retests throughout the week. |
| Slideshow takes longer than expected | Break the work into manageable tasks and review scope without dropping essential checks. |
| Client photos or contact details are sensitive | Confirm permission before placing them in a public repository or publishing them. |
| Outstanding Sprint 0 questions affect later work | Keep their next actions in the carry-forward backlog; do not treat them as resolved by the homepage build. |

## 7. Order and dependencies

1. Check the requirements, assets and approvals.
2. Build the homepage structure and shared layout.
3. Add content and homepage features.
4. Test as work progresses, then complete checks and retests.
5. Review the outcome and record the retrospective.

Keep no more than two cards active at once and use one branch per card.

## 8. Timeline

### Dates

| Item | Date |
|---|---|
| Start | To confirm |
| Planned end | To confirm — one week after start, subject to my schedule |
| Available hours | To confirm |

### Hours

| Card | Planned hours | Target date | Actual hours | Notes |
|---|---:|---|---:|---|
| 1. Prepare homepage content | To estimate | To confirm | | |
| 2. Build homepage structure | To estimate | To confirm | | |
| 3. Add homepage content and features | To estimate | To confirm | | |
| 4. Test and improve homepage | To estimate | To confirm | | Include retesting |
| 5. Review Sprint 1 | To estimate | To confirm | | |
| **Total** | **To estimate** | | | |

## 9. Review

*Complete at the end of the sprint using actual evidence.*

| Item | Entry |
|---|---|
| Date | |
| Goal vs outcome | |
| Completed work and evidence | |
| Incomplete work and next action | |
| Client feedback, if received | |

| Merit criterion | Evidence and current status |
|---|---|
| To check against the supplied specification | |

## 10. Retrospective

*Complete at the end of the sprint.*

**What went well**

**What to change**

**One action for the next sprint**

## 11. Carry-forward backlog

| Item | Next action | Status |
|---|---|---|
| Enquiry privacy and data handling | US05 includes a required full-address field. Before enabling submissions, verify the form provider, recipients/processors, access and protection, retention and deletion, and contact route. Make accurate privacy information accessible from the form, footer and FAQ. | Before form submissions |
| Consultation flow | Confirm whether the form starts the consultation or Lydia follows up separately | Open |
| Hosting, domain, service and maintenance costs | Verify costs and arrangements before the relevant build or launch decision | Open |
| Services & Prices page | Build and test in its own page sprint | Planned |
| Enquiry page and form | Build in its own page sprint; verify data handling before enabling submissions | Planned |
| Reviews page | Build and test separately from the homepage review carousel | Planned |
| Gallery page | Build and test in its own page sprint; confirm Instagram feasibility, with hand-built fallback | Planned |
| FAQ page | Build and test in its own page sprint | Planned |
| Integration, deployment and handover | Test cross-page behavior, deploy and complete project documentation after page sprints | Planned |
| Other unfinished Sprint 1 work | Add items and next actions at sprint review | To record |