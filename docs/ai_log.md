# AI log

**About the dates and evidence in this log**
- No screenshot shows an absolute date. They show clock times (for example 7:07 PM) or relative times (for example "12 hours ago" in the Claude screenshots). Dates in this log come from my own record and from the git commit history. Git first records these files on 27/10/2026, because the Sprint 0 documents were split into separate commits that day (see Entry 4).
- Where a screenshot does not show the model, this log says so.
- This log was written and edited with AI assistance in places. Copilot wrote the text of Entry 6 at my request (see Entry 6), and Copilot Chat helped correct this log against my screenshots on 29/10/2026.

## Entry 1: Defining AI working rules and handover document (hbl-ai-rules.md)

**Date(s):** 26/10/2026 (from my own record; the screenshots show times only, 7:07 PM to 7:42 PM, and git first records these files on 27/10/2026)  
**Tool:** Copilot Chat in VS Code (the model is shown as `Auto (gpt-6-luna)` in `ai_rules7.png` and `handover-duplicate-example.png` only; it is not shown in the other screenshots)  
**Reference:** GitHub (2026) *GitHub Copilot Chat* [Generative AI] Available from https://github.com/features/copilot [Accessed 26 October 2026].  
**Purpose:** To set working rules for how an AI assistant mentors and reviews my Hair by Lydia project without authoring my assessed work.

### Interaction record

| # | What I asked | What the AI returned | Evidence |
|---|---|---|---|
| 1 | I supplied 12 proposed working rules (single-item commits, two-item work limit, project board, testing and evidence, hints not full code, Definition of Done, tests before work, traceability, retrospectives, rejected options, client input logged, no catch-up commits). | A review citing criteria 4.2, 5.1, 5.2 and M(iv)/M(vii), flagging a risk of administrative overload. | [ai_rules2.png](screenshots/ai_rules2.png) and [ai_rules3.png](screenshots/ai_rules3.png) show my 12 rules and the review. [ai_rules1.png](screenshots/ai_rules1.png) shows an AI-facing "Copilot instructions" prompt at the start of the session. That prompt is for the AI's use only. It is kept outside this repository and is not part of the submitted project. It states that earlier documents in `docs/` were partly AI-drafted. |
| 2 | I asked it to explain everything expected of it, whether it would remember the context, and how to enforce the rules. | An explanation of its role, hint levels and evidence handling. It said it could not guarantee memory across sessions. | [ai_rules4.png](screenshots/ai_rules4.png) (my question), [ai_rules5.png](screenshots/ai_rules5.png) (the explanation) |
| 3 | I asked it to define each behaviour rule by number. | A numbered breakdown of how it would apply my 12 rules. | [ai_rules5.png](screenshots/ai_rules5.png) (my request), [ai_rules6.png](screenshots/ai_rules6.png) (the breakdown) |
| 4 | I proposed dated session handover documents and said they were for AI agents only, so it could generate them outright. | It recommended separating the stable rules from dated handovers and using lowercase filenames (criterion 3.8). I clarified that AI-facing documents could be generated with my authorisation. The screenshots record this discussion and naming guidance, not a completed session handover. | [ai_rules7.png](screenshots/ai_rules7.png) (naming guidance, my reply that AI-facing documents could be generated, and the model `Auto (gpt-6-luna)` at 7:27 PM) |
| 5 | I asked why the AI-facing rules contained two session-end handover sections. | The AI acknowledged that it had introduced the duplicate sections and offered to merge them. I checked the content and removed the duplicate myself, taking care not to remove relevant information. | [handover-duplicate-example.png](./screenshots/handover-duplicate-example.png) |
| 6 | I asked for the framework to cover all project stages, not only Sprint 0. | A lifecycle-wide planning and workflow section, which Copilot proposed as replacement text for the draft. | [ai_rules8.png](screenshots/ai_rules8.png) (my request, and the end of the draft), [ai_rules9.png](screenshots/ai_rules9.png), [ai_rules10.png](screenshots/ai_rules10.png) (the replacement section) |
| 7 | I asked for my appendix draft in Markdown. | My draft reformatted, noted as unverified. | [appendix_markdown_result.png](screenshots/appendix_markdown_result.png) |

### Project documents
- [hbl-ai-rules.md](hbl-ai-rules.md): the resulting AI-facing rules (AI-assisted)
- [appendix.md](appendix.md): my AI disclosure draft
- [ai_log.md](ai_log.md): this log

### My decisions

**Accepted**
- I adopted the Merit criteria review checkpoint and the appendix-planning elements the AI suggested. (Evidence: appendix.md, section 2.)
- I accepted separating the stable rules file (`hbl-ai-rules.md`) from dated session handovers, and I accepted the AI's point that criterion 3.8 requires lowercase filenames with no spaces. (Evidence: ai_rules5.png.)
- I accepted a lifecycle-wide planning and workflow section after I asked for the framework to cover all stages, not only Sprint 0. This kept the rule that Sprints 0 and 0.5 are planned in detail and later sprints stay at theme level until the Sprint 0.5 review. (Evidence: ai_rules6.png to ai_rules10.png, hbl-ai-rules.md.)
- I accepted the session-end handover section and the evidence-first rules: no claim that work happened without dated evidence, and "INSUFFICIENT CONTEXT" when information is missing. (Evidence: hbl-ai-rules.md.)

**Changed**
- I decided the AI-facing documents did not need designing by me and could be generated by the AI, because they are for AI agents only. This changed my earlier rule that the AI never creates or edits files. At the time, the rules file limited the exception to AI-facing behaviour and session-handover documents, and only where I authorised it. (Evidence: ai_rules5.png; the "Role and authorship" section of hbl-ai-rules.md.)
- I changed the plan-first rule so the AI will not propose a final plan before I have drafted one, except where I explicitly request an exception for an AI-facing document. (Evidence: hbl-ai-rules.md, "Mentoring and review".)
- I identified a duplicate handover section and had it removed. (Evidence: handover-duplicate-example.png.)
- I kept all 12 of my original rules as written and expanded them to be stricter and to cover fallbacks. (Evidence: hbl-ai-rules.md.)

**Rejected**
- The AI warned that “a card for every new work action” and recording every small design decision could create administrative overload. I kept those rules, because they give me dated, traceable evidence for the assessment criteria Copilot cited (4.2, 5.1 and 5.2), and I manage the overhead with the two-item work limit. The final file has them as “cards with acceptance criteria” and a decision log. (Evidence: hbl-ai-rules.md, rules 3 and 4; ai_rules1.png to ai_rules3.png.)
- The AI suggested I write the working rules in my own words. I chose to have it generate the AI-facing text instead, because the document is for AI agents only.

### Where this was used
- `hbl-ai-rules.md`: AI-assisted project document.
  - **My ideas and wording:** the 12 working rules I supplied (single-item commits, two-item work limit, project board, testing and evidence, hints not full code, Definition of Done, tests before work, traceability, retrospectives, rejected options, client input logged, no catch-up commits). The decision that AI-facing documents can be generated by the AI where I authorise it, and the rule that the AI does not propose a final plan before I have drafted one, are also mine.
  - **Drafted or structured by Copilot:** the separation of stable rules from dated session handovers, the lowercase filenames, the lifecycle-wide planning and workflow section, the session-end handover section, and the evidence-first rules (no claim without dated evidence, "INSUFFICIENT CONTEXT" when information is missing).
  - **Corrected by me:** Copilot introduced a duplicate session-end handover section. I checked the content and   removed the duplicate myself.

  ### Limits of this evidence
- The AI-facing rules file shows the project's AI boundaries. It does not show that the rules were followed.
- Screenshots are stored in `docs/screenshots/` and linked above. Confirm that the assessor can access the folder before submission.

### My responsibility
I made the project decisions. The AI structured and drafted the AI-facing rules text at my request.

## Entry 2: Q1–Q26 requirements mapping (Copilot)

**Date(s):** 27/10/2026  
**Tool:** Copilot Chat in VS Code (the model and date are not shown in the screenshots)  
**Reference:** GitHub (2026) *GitHub Copilot Chat* [Generative AI] Available from https://github.com/features/copilot [Accessed 27 October 2026].  
**Purpose:** To work through Lydia's completed client questionnaire, which I designed with Jesse James Garrett's planes of user experience in mind, and to use Copilot's framework to map her answers (Q1–Q26) to needs, features, source tags and gaps, without Copilot authoring the table for me.

### Interaction record

| # | What I asked | What the AI returned | Evidence |
|---|---|---|---|
| 1 | I asked it to act as an interactive project mentor and work through the Q1–Q26 mapping in small batches (starting with Q1 to Q5), without generating the full table or inventing my interpretations. For each batch it was to state what Lydia said, ask for my interpretation [P], derived need or feature, source tag and gap to ask Lydia, and wait for my response. | It read the questionnaire and my sprint plan, then asked for a mapping for each question in turn using that framework. It did not provide example answers. | [questionaire-requirements-mapping-1.png](screenshots/questionaire-requirements-mapping-1.png), [questionaire-requirements-mapping-2.png](screenshots/questionaire-requirements-mapping-2.png) |
| 2 | I submitted an answer for each question (Q1–Q26) in the four-part format. The answers were adapted from example answers drafted with another AI tool (see Entry 3). For Q19 I first submitted the Q18 answer by mistake and then sent a correction. | It recorded each answer against its question and moved on to the next. | [questionaire-requirements-mapping-2.png](screenshots/questionaire-requirements-mapping-2.png) (Q1–Q13), [questionaire-requirements-mapping-3.png](screenshots/questionaire-requirements-mapping-3.png) (Q13–Q26) |
| 3 | I completed the Q21–Q26 batch. | It confirmed Q21–Q26 from my mappings and listed boundaries to preserve (for example, permission to post online may not cover the website, and Instagram sourcing and the update process stay [P]/[C] pending research). It said the discussion was complete without assembling the full table. | [questionaire-requirements-mapping-1.png](screenshots/questionaire-requirements-mapping-1.png) |

### Project documents
- [questionaire-hbl.md](questionaire-hbl.md): questionnaire and Lydia's answers
- [requirements-mapping.md](requirements-mapping.md): Q1–Q26 mapping (card 1 evidence, AI-assisted)

### My decisions

**Accepted**
- I used the four-part answer format from my mentor prompt (interpretation [P], derived need or feature, source tag, gap to ask Lydia) for every row. (Evidence: questionaire-requirements-mapping-2.png, requirements-mapping.md.)
- The final Q21–Q26 rows keep the boundaries Copilot listed: website permission is not assumed, Instagram sourcing and the update process are [P]/[C] pending research, and costs are researched rather than estimated. (Evidence: questionaire-requirements-mapping-1.png, requirements-mapping.md rows Q21–Q26.)

**Changed**
- I adapted the example answers from Entry 3, including the rows revised at my direction (Q11, Q13, Q17, Q21, Q24, Q26), before submitting them, and compiled the confirmed rows into the Q1–Q26 table. (Evidence: questionaire-requirements-mapping-2.png, questionaire-requirements-mapping-3.png, requirements-mapping.md.)
- I noticed that I had submitted the Q18 answer for Q19 and corrected it. (Evidence: questionaire-requirements-mapping-3.png.)

**Rejected**
- None recorded.

### Where this was used
- `requirements-mapping.md`: AI-assisted project document. Copilot provided the framework, asked the questions and checked my answers. The answer wording was adapted from drafts recorded in Entry 3.

### Limits of this evidence
- The screenshots show each question and the start of each answer. The full answers are in `requirements-mapping.md`.
- The submitted answers closely follow the example answers in Entry 3, so they are adapted from AI drafts, not written independently.
- The mapping is my analysis, produced with AI assistance. It is not Lydia's confirmation of it.
- Screenshots are stored in `docs/screenshots/` and linked above. Confirm that the assessor can access the folder before submission.

### My responsibility
I made the project decisions, adapted the example answers and submitted them to Copilot. Copilot provided the framework and checked my answers. The example answers and revisions I directed are recorded in Entry 3.

## Entry 3: Example answers and revisions for the Q1–Q26 requirements mapping (Claude)

**Date(s):** 27/10/2026  
**Tool:** Claude Sonnet 5.5 (Anthropic) via the claude.ai web app (the model name is visible in `questionaire-requirements-mapping-13.png` only; the screenshots show relative times such as "12 hours ago", not dates)  
**Reference:** Anthropic (2026) *Claude Sonnet 5.5* [Generative AI] Available from https://claude.ai [Accessed 27 October 2026].  
**Purpose:** To provide example answers in the four-part mapping format for me to adapt, to revise specific rows to include my ideas, and to format the finished table as markdown.

### Interaction record

| # | What I asked | What the AI returned | Evidence |
|---|---|---|---|
| 1 | I used the same mentor approach as in Entry 2, then asked it to give its own answers to its questions as a template for how to answer, and gave it my summaries of Q6–Q26 batch by batch. | Full example answers in the four-part format (interpretation, derived need or feature, source tag, gap) for the batches shown in the screenshots. The screenshots do not capture the original drafts for Q14–Q15, Q18–Q20 or Q23–Q26 (my revisions to Q24 and Q26 are shown). | [questionaire-requirements-mapping-4.png](screenshots/questionaire-requirements-mapping-4.png) (Q1–Q5), [5](screenshots/questionaire-requirements-mapping-5.png), [6](screenshots/questionaire-requirements-mapping-6.png), [7](screenshots/questionaire-requirements-mapping-7.png) (Q6–Q10), [8](screenshots/questionaire-requirements-mapping-8.png) (Q11–Q13), [11](screenshots/questionaire-requirements-mapping-11.png) (Q16–Q17), [13](screenshots/questionaire-requirements-mapping-13.png) (Q21–Q22) |
| 2 | I told it what to change in specific rows: a form-to-email enquiry flow, pulling gallery images from Lydia's Instagram, building on her existing systems so maintenance is minimal, and keeping running costs low or free where possible. I also asked whether photo attachments would need a backend. | Revised rows (Q11, Q13, Q17, Q21, Q24, Q26) that included my ideas, tagged them as proposals to confirm, and flagged feasibility questions for my research card. It confirmed that photo uploads would need a form service or backend. | [Q11](screenshots/questionaire-requirements-mapping-9.png), [Q13](screenshots/questionaire-requirements-mapping-10.png), [Q17](screenshots/questionaire-requirements-mapping-12.png), [Q21](screenshots/questionaire-requirements-mapping-14.png), [Q24](screenshots/questionaire-requirements-mapping-15.png) and [its email revision](screenshots/questionaire-requirements-mapping-16.png), [Q26](screenshots/questionaire-requirements-mapping-17.png) |
| 3 | I pasted my completed Q1–Q26 table and asked it to present it as markdown to match my existing work. | A formatted `requirements-mapping.md` with a header and source key. It changed one spelling ("behavior" to "behaviour") and replaced curly quotes with plain ones. It did not change the content. |[questionaire-requirements-mapping-19.png](screenshots/questionaire-requirements-mapping-19.png) |

### Project documents
- [requirements-mapping.md](requirements-mapping.md): Q1–Q26 mapping (card 1 evidence, AI-assisted)

### My decisions

**Accepted**
- I used the four-part format and the [Q]/[P]/[C] source tags in the example answers. (Evidence: requirements-mapping.md.)

**Changed**
- I adapted the example answers into my own answers for Copilot's questions (see Entry 2).
- I directed a form-to-email enquiry flow, and treated photo upload as a feasibility question because attachments would need a form service or backend. (Evidence: requirements-mapping.md rows Q11 and Q17; questionaire-requirements-mapping-9.png, questionaire-requirements-mapping-12.png.)
- I directed pulling gallery images from Lydia's Instagram, subject to research, with a manual-update fallback. (Evidence: requirements-mapping.md rows Q13 and Q21.)
- I directed building on systems Lydia already uses so maintenance is minimal, and aiming for low or free running costs where possible. (Evidence: requirements-mapping.md rows Q24 and Q26.)

**Rejected**
- None recorded.

### Where this was used
- `requirements-mapping.md`: AI-assisted project document. Claude's example answers were used as a model for wording and level of detail, and Claude formatted the final table as markdown.
- The form-to-email flow, Instagram-sourced gallery, existing-systems principle and low-cost aim are my ideas. The AI added them to the rows at my direction.

### Limits of this evidence
- Several final rows follow the structure and wording of the example answers closely, so they are adapted from AI drafts, not written independently.
- The mapping is my analysis, produced with AI assistance. It is not Lydia's confirmation of it.
- The Claude screenshots show "Added to memory hair-by-lydia.md", so Claude kept a project memory file during these sessions. The screenshots also show Claude creating `requirements-mapping.md` itself in the formatting step.

### My responsibility

I made the project decisions and directed the changes to the mapping. Claude drafted example answers that I adapted, revised rows at my direction and formatted the final table.

## Entry 4: Review and revision of AI disclosure (Copilot)

**Date:** 27/10/2026  
**Tool:** Copilot Chat in VS Code, auto-routed to Claude Sonnet 5.5 (shown in `questionaire-requirements-mapping-18.png` as "Auto routed task to Claude Sonnet 5.5", 4:23 PM)  
**Reference:** GitHub (2026) *GitHub Copilot Chat* [Generative AI] Available from https://github.com/features/copilot [Accessed 27 October 2026].  
**Purpose:** To review whether my appendix accurately described my AI use and make the disclosure more complete and concise.

### Interaction record

| # | What I asked | What the AI returned | Evidence |
|---|---|---|---|
| 1 | I asked how to make the appendix accurate, then asked for exact wording based on my current evidence and AI log. | It identified that the appendix did not clearly disclose Claude's example answers and formatting for the Q1–Q26 mapping, Copilot's question-by-question guidance, and AI assistance with the disclosure itself. It suggested replacement wording and evidence-list changes. | Current Copilot conversation transcript. |
| 2 | I asked Copilot to make the proposed changes. | It updated the appendix to describe the AI contributions, distinguish actual use from intended safeguards, and state that reference details and assessor access to the evidence still need to be checked before submission. | `docs/appendix.md`; current Copilot conversation transcript. |
| 3 | I asked it to review the disclosure again, then asked what evidence I should collect and shared my screenshots of the Claude and Copilot sessions. | It first suggested that Copilot assembled the mapping wording from my independent answers. The screenshots showed that the wording started as Claude drafts, so it corrected that and advised grouping the screenshots by tool and step, adding dates, and fixing broken evidence links in this log. | [questionaire-requirements-mapping-18.png](screenshots/questionaire-requirements-mapping-18.png) |

### My decisions

**Accepted**
- I authorised the appendix changes, including disclosure that this review contributed wording to the appendix.

**Changed**
- I did not accept the earlier suggestion that the mapping wording was mine alone, because my screenshots show it started as Claude drafts. The appendix and Entries 2 and 3 say so.
- I corrected screenshot links in Entries 2 and 3 after the review.

**Rejected**
- None recorded.

### Where this was used

- `docs/appendix.md`: revised AI disclosure draft.

### Version control note

On 27/10/2026, the Sprint 0 documents were first committed together and then split into one commit per item before the first push to GitHub. Copilot helped me run the git commands for the split. Commit dates reflect the split, not when each item was written.

### Limits of this evidence

- The transcript records the review and requested changes; it is not an institute-issued AI reference.
- Only `questionaire-requirements-mapping-18.png` captures this session. It shows my prompt "how would these screenshots help" and the response, not the earlier appendix-rewrite exchanges (rows 1 and 2). Those are recorded in this entry and in the git history of `docs/appendix.md`, and I have no screenshots of them.
- The Copilot model route (Claude Sonnet 5.5) is known for this screenshot only. This is an example of Copilot auto-routing to different models, so other Copilot entries may also have used models that are not shown.
- Assessor access to the `docs/screenshots/` folder still needs checking before submission.

## Entry 5: Competitor research guidance, feedback and copy-edit (Copilot)

**Date:** 27/10/2026  
**Tool:** Copilot Chat in VS Code (Copilot SDK)  
**Reference:** GitHub (2026) *GitHub Copilot Chat* [Generative AI] Available from https://github.com/features/copilot [Accessed 27 October 2026].  
**Purpose:** To get guidance on the competitor research card, then have my write-up reviewed and copy-edited.

### Interaction record

| # | What I asked | What the AI returned | Evidence |
|---|---|---|---|
| 1 | I asked whether to make the checklist and research note a markdown file to link as evidence. | Advice to use one file, `docs/competitor-research.md`, with suggested sections: purpose and method, a checklist table, per-site notes with URL, date accessed and linked screenshots, adopt or avoid takeaways, open questions tagged [C], and an AI-use line. It said to tag assumptions [P] and open questions [C]. It also advised one commit per item. (Timestamp in the screenshot: 8:53 PM.) | [competitor-research-markdown-ai-4.png](screenshots/competitor-research-markdown-ai-4.png) |
| 2 | I asked for help with the competitor research card (#3). | Tips for the task: pick three comparable sites, use one checklist for each (layout, gallery, prices, enquiry route, mobile and basic accessibility), score each Yes, Partial or No with a one-line note, save dated screenshots, record each takeaway as adopt or avoid, save the file as `docs/competitor-research.md`, and log AI use. It offered to help build the checklist table or review my findings, and said it would not write the analysis. | [competitor-research-markdown-ai-3.png](screenshots/competitor-research-markdown-ai-3.png) |
| 3 | I asked it to review my competitor research and give feedback. | General feedback on structure and evidence, for example defining the source tags and matching each screenshot to the claim it supports. | [competitor-research-markdown-ai-1.png](screenshots/competitor-research-markdown-ai-1.png) |
| 4 | I asked it to apply smaller edits where needed and check spelling and grammar. | Edits to `competitor-research.md` that corrected spelling and grammar, standardised British spelling, made headings consistent and tightened some wording. For example, "live navigation indicator" became "active-section indicator". | [competitor-research-markdown-ai-2.png](screenshots/competitor-research-markdown-ai-2.png); `docs/competitor-research.md` |

### Project documents
- [competitor-research.md](competitor-research.md): competitor research
- [lydia-competitor-rough-notes.txt](lydia-competitor-rough-notes.txt): my raw notes from the first review with Lydia

### My decisions

**Accepted**
- I used the checklist areas and the Yes, Partial or No scoring from the guidance, and the suggested single markdown file.
- I accepted the spelling, grammar and consistency edits.

**Changed**
- I built the markdown document myself around the checklist, and entered Lydia's feedback and my own observations, scores and assumptions.
- I used one table for each competitor with a score column and a one-line note, instead of the single table with a column for each site that was suggested.
- After the feedback recommended defining the source labels, I added a source key adapted from the one in `requirements-mapping.md`.
- I treated the feedback as advice. I did not add new research requirements, and I decided the research was sufficient for my needs.

**Rejected**
- None recorded.

### Where this was used
- `competitor-research.md`: the file name, suggested sections, checklist areas and scoring scale came from Copilot's guidance. Spelling, grammar, British spelling, heading consistency and some rewording were Copilot's edits. The observations, scores, takeaways and decisions are mine.

### Version control note
Commit `7a91d2d` ("Add competitor research documentation") has a `Co-authored-by: Copilot` trailer. Copilot added it by default when it suggested the commit command, and I did not ask for it. It does not mean Copilot wrote the research content.

### Limits of this evidence
- I have no screenshot or transcript showing Copilot supplying a ready-made markdown table. The screenshots show guidance on structure and checklist areas only, so I describe the table layout as my own.
- The screenshots show the start of each response and the copy-edit summary, not the full conversations.
- `competitor-research-markdown-ai-3.png` (row 2) shows the response only. My prompt for it is not visible in that screenshot, so row 2 is my description of what I asked.
- Times in these screenshots (8:53 PM, 9:54 PM, 9:57 PM) have no dates. The models are not shown.
- The transcript is not an institute-issued AI reference.
- The research is my own analysis from Lydia's feedback and my visits to the websites. Lydia has not confirmed my assumptions.

### My responsibility
I chose and visited the competitors, entered Lydia's feedback, made the observations and scored the sites. Copilot gave guidance, reviewed the write-up and copy-edited it at my request, and I decided what to keep.

## Entry 6: Feature research document from rough notes (Copilot)

**Date:** 29/10/2026
**Tool:** Copilot Chat in VS Code (Copilot SDK)
**Reference:** GitHub (2026) *GitHub Copilot Chat* [Generative AI] Available from https://github.com/features/copilot [Accessed 29 October 2026].
**Purpose:** To turn my feature research rough notes into a final Markdown research and decision log, record a dated client agreement, and link the document as Sprint 0 evidence.

### Interaction record

| # | What I asked | What the AI returned | Evidence |
|---|---|---|---|
| 1 | I asked it to convert my rough feature-research notes into a final Markdown document saved in the repository, add [P] and [C] tags, write a dated note of what Lydia agreed on 28/10/2026, and add an AI log entry. | A structured feature research and decision log in `docs/feature-research.md`, with proposals and outstanding checks labelled. It recorded Lydia's agreement to drop the transparent header in favour of a taupe fixed header, as stated in my rough notes, and linked the document from the Sprint 0 evidence table. It did not independently verify the research sources or the client discussion. | This Copilot Chat transcript (29 October 2026); [original rough notes](../notes/features-research-rough-notes.txt); [feature research document](feature-research.md); [Sprint 0 plan](../sprints/sprint-0.md); [completion screenshot](screenshots/feature-research-completion.png). |

### Project documents
- [feature-research.md](feature-research.md): feature research and decision log converted from my rough notes
- [sprint-0.md](../sprints/sprint-0.md): evidence link for the research card
- [features-research-rough-notes.txt](../notes/features-research-rough-notes.txt): original notes retained as source evidence
- [feature-research-completion.png](screenshots/feature-research-completion.png): screenshot of the request and completed changes

### My decisions

**Recorded from my notes**
- I recorded the header decision as Lydia's agreement to drop the transparent effect and use a taupe fixed header from the top of the page, dated 28/10/2026.

**Limits**
- Copilot wrote the text of this log entry at my request (my prompt asked it to add an AI log entry; `feature-research-completion.png` shows it recorded the work in `ai_log.md`). I have reviewed it. The model and the date are not shown in that screenshot.
- The screenshot shows my request and the completion summary only, not the full conversation.
- The AI edited and organised the notes, but did not independently verify their external sources, test the proposed services, or witness Lydia's discussion. The dated client note is based on my rough notes.

## Entry 7: Approach update and revised AI workflow

**Date:** 29/10/2026  
**Tool:** Copilot Chat in VS Code  
**Purpose:** To reflect on how my AI use has developed, update my working rules to match my actual practice, and stop using session handovers.

### Approach update

Reviewing this log made me recognise that my use of AI has developed beyond my original plan for AI to act only as a mentor and reviewer. Later entries record AI assistance with drafting, structuring and reviewing project documents. I have updated my working rules to reflect my actual use: I may ask AI to help with project documents, while remaining responsible for reviewing and adapting the work, checking facts and sources, understanding the final material, and acknowledging AI contributions accurately.

I no longer use session handovers. I often forgot to generate one at the end of a session, so handovers were not a reliable way to maintain project context. I will continue to apply my AI-use rules when using AI for project work and record its contributions, my decisions and the checks I make. I remain responsible for my project decisions and for ensuring my AI use follows the applicable course requirements.

### Interaction record

| # | What I asked | What the AI returned | Evidence |
|---|---|---|---|
| 1 | I asked for a critical review of my AI-use approach, then authorised updating the rules, moving this approach update out of Entry 1, and aligning the disclosure citations. | It identified the mismatch between my original rules and later documented AI use, recommended a dated update, and made the authorised changes. | Current Copilot Chat transcript (29 October 2026); this entry and the revised [AI rules](hbl-ai-rules.md) and [appendix](appendix.md). |

### My responsibility

I recognised the change in my practice and decided to stop using handovers because I often forgot to prepare them. I authorised the rule and disclosure updates, reviewed the changes, and remain responsible for applying the rules and accurately disclosing AI use.

## Entry 8: Design principles and accessibility notes formatted as Markdown (Copilot)

**Date:** 31/10/2026
**Tool:** Copilot Chat in VS Code (Copilot SDK)
**Reference:** GitHub (2026) *GitHub Copilot Chat* [Generative AI] Available from https://github.com/features/copilot [Accessed 31 October 2026].
**Purpose:** To format my design-principle rough notes as Markdown without changing their wording, retain the original draft as evidence, and record the AI assistance.

### Interaction record

| # | What I asked | What the AI returned | Evidence |
|---|---|---|---|
| 1 | I asked it to reformat my design-principle rough notes as Markdown without changing any wording, keep the original draft for evidence, record the work in the AI log, and not commit anything. | A Markdown-formatted copy of the notes, with the original rough-notes file left unchanged. | [Screenshot of my request and completion summary](screenshots/design-principles-formatting-completion.png); [original rough notes](../notes/design-principles-accessibility-rough-notes.txt); [formatted document](design-principles-accessibility.md). |

### Project documents
- [design-principles-accessibility.md](design-principles-accessibility.md): Markdown-formatted copy of the design-principle and accessibility notes
- [design-principles-accessibility-rough-notes.txt](../notes/design-principles-accessibility-rough-notes.txt): original draft retained unchanged as evidence
- [design-principles-formatting-completion.png](screenshots/design-principles-formatting-completion.png): screenshot of the request and completion summary

### My decisions

**Accepted**
- I kept the original rough notes unchanged and added the Markdown version as a separate document.
- I asked for the wording to remain unchanged; the changes are Markdown formatting only.

**Rejected**
- None recorded.

### Limits of this evidence
- The screenshot shows the request and completion summary, not the full conversation or the contents of the resulting files.
- No commit was made as part of this edit.

## Entry 9: Wireframe review and enquiry-field update (Copilot)

**Date:** 05/11/2026
**Tool:** Copilot Chat in VS Code (Copilot SDK)
**Reference:** GitHub (2026) *GitHub Copilot Chat* [Generative AI] Available from https://github.com/features/copilot [Accessed 5 November 2026].
**Purpose:** To review the wireframes against the project guide and existing project work, and record the user's decisions and the requested enquiry-field correction.

### Interaction record

| # | What I asked | What the AI returned | Evidence |
|---|---|---|---|
| 1 | I asked it to review my wireframes against the project guide and existing work. | It identified possible inconsistencies and omissions in the About page, enquiry fields and states, carousel controls, hero slideshow, FAQ, and gallery alt text. | [Screenshot of my review request and summary](screenshots/wireframe-review-summary.png); current Copilot Chat conversation (5 November 2026); [wireframes](wire-frames.md). |
| 2 | I clarified that About content is being incorporated into the homepage; that the slowly rotating review carousel should let users pause it; and that the hero design is my choice, discussed with Lydia. I also said Instagram-provided images should have before/after alt text if a hand-built gallery is used. I asked it to correct the enquiry fields. | It changed the mobile and desktop enquiry wireframes to show phone as required, email as optional, and address/location details and requiredness as needing confirmation. It made no other wireframe changes. | [Screenshot of my decisions and the enquiry-field update](screenshots/wireframe-review-decisions.png); current Copilot Chat conversation (5 November 2026); [wireframes](wire-frames.md). |
| 3 | I asked Copilot to record the interaction in the appendix and AI log. | It added this entry and updated the appendix disclosure. | [Screenshot of my logging request and completion summary](screenshots/wireframe-review-log-update.png); current Copilot Chat conversation (5 November 2026); [appendix](appendix.md). |

### Project documents
- [wire-frames.md](wire-frames.md): enquiry-field labels updated in the mobile and desktop wireframes
- [appendix.md](appendix.md): disclosure of this AI-assisted review and the user's decisions

### Screenshots
- [wireframe-review-summary.png](screenshots/wireframe-review-summary.png): review request and summary
- [wireframe-review-decisions.png](screenshots/wireframe-review-decisions.png): user's clarifications and the enquiry-field update
- [wireframe-review-log-update.png](screenshots/wireframe-review-log-update.png): request to record the interaction and completion summary

### My decisions and responses to AI suggestions

**Accepted**
- I accepted the enquiry-field correction: phone is required, email is optional, and the address/location field's detail and requiredness still need confirmation. Copilot updated the mobile and desktop wireframes accordingly.

**AI suggestions not adopted**
- Copilot suggested adding a separate About page and corresponding navigation/footer links. I did not adopt this because the About content is being incorporated into the homepage.
- Copilot recommended that the reviews carousel not auto-rotate. I chose slow rotation with user controls to pause it.
- Copilot suggested making the hero slideshow conditional or using a static fallback until approval. I chose the hero design after prior discussion with Lydia.

**Clarification**
- Copilot suggested distinct before-and-after image descriptions. Instagram-sourced images will use Lydia's Instagram content; if I hand-build the gallery, I will add suitable alt text for before-and-after images.

**Other suggestions**
- I made no further wireframe changes in response to the remaining review suggestions during this interaction.

### Limits of this evidence
- This entry records the current conversation and the resulting enquiry-field edit; it does not establish that the discussed design choices have been implemented or tested.

## Entry 10: Website brief revised from rough notes (Copilot)

**Date:** 5/11/2026

**Tool:** Copilot Chat in VS Code. The first review used GPT-6 Luna (shown in the screenshot). Later turns, including drafting the brief and this entry, were handled by Claude Sonnet 5.5 (stated by the assistant in the conversation; no screenshot shows this).

**Reference:** GitHub (2026) *GitHub Copilot Chat* [Generative AI] Available from https://github.com/features/copilot [Accessed 5 November 2026].

**Purpose:** To review my rough website brief against my existing project documents, put questions to me about open wording and decisions, prepare a Markdown brief from my rough notes and answers, and record my decisions about the review.

**Authorship:** Copilot drafted the text of `docs/brief.md` and of this entry at my request. The ideas, decisions and answers come from my rough notes and my replies; the wording is Copilot's. I will ask my assessor how this AI-drafted material may be used and evidenced. Rewording it does not by itself establish that it is independently produced work.

### Interaction record

| # | What I asked | What the AI returned | Evidence |
|---|---|---|---|
| 1 | I asked how I could improve my rough website brief into a finalised version. I then clarified that deposits are upon request; Lydia aims to reply within two working days; 25 December remains the deadline, with a grace period through 1 January if needed. I asked the AI to ask me about unresolved edits and changes, reflect what I kept, rejected or changed, update the AI log, and reference my rough notes as evidence. | Copilot reviewed the rough notes against the existing brief-related project documents, asked me questions (shown in the screenshot of my answers), then created a new `docs/brief.md` while retaining the rough notes as source evidence. It incorporated my corrections, kept my proposals distinct from Lydia's input, and recorded remaining checks without claiming Lydia had reviewed or signed off the brief. | [Original rough notes](../notes/brief-rough-note.txt); [new website brief](brief.md); current Copilot Chat conversation (5 November 2026); [screenshot of my review request and the initial review](screenshots/brief-review-request.png); [screenshot of the questions and my answers](screenshots/brief-question-answers.png); [screenshot of my logging request and completion summary](screenshots/brief-log-update.png). |

### Project documents

- [brief.md](brief.md): new Markdown website brief prepared from my rough notes
- [brief-rough-note.txt](../notes/brief-rough-note.txt): original rough notes retained as evidence
- [brief-review-request.png](screenshots/brief-review-request.png): my review request and the AI's initial review
- [brief-question-answers.png](screenshots/brief-question-answers.png): the questions Copilot asked and my answers (the right edge of the longest answer is cropped)
- [brief-log-update.png](screenshots/brief-log-update.png): my logging request and completion summary
- [user-stories.md](user-stories.md), [feature-research.md](feature-research.md), [wire-frames.md](wire-frames.md), [lydia-feedback.md](lydia-feedback.md) and [questionaire-hbl.md](questionaire-hbl.md): documents checked for consistency

### My decisions and responses to AI suggestions

**Kept or confirmed**

- I confirmed that deposits may be required upon request.
- I confirmed the project deadline remains 25 December 2026, with a grace period through 1 January 2027 if needed.
- I confirmed that the proposed usability targets are intended goals and should not make the design harder. (Evidence: [my answers](screenshots/brief-question-answers.png).)
- I kept the hero slideshow after tweaking it and speaking to Lydia, and I will build a fallback if Instagram fails. My answer also mentions the About page at Lydia's request, but that part is cropped in the screenshot, so I am not relying on it here.
- I answered that the brief should be a fresh `docs/brief.md`, with the existing files kept as evidence and linked. The original rough notes remain in place.
- I answered "Correct" when asked to confirm that the brief should use my voice and approval status. I understand now that Copilot wrote the wording; I will check with my assessor how to use it.
- I stated that January 1st is a grace period if needed.

**Changed or clarified**

- I corrected the response-time wording to say that Lydia aims to reply within two working days. When asked about it, I answered that this conversation with Lydia is not recorded because I do not keep a log of every conversation. It is therefore my account only. On 8 November, I explained that I had suggested up to two working days to give Lydia breathing room and decided to use Lydia's own wording instead: she usually aims to reply within one working day. The earlier questionnaire and current user story reflect that wording.
- I corrected the earlier review's deposit wording: deposits are upon request.
- I said 25 December remains the deadline, with 1 January as a grace period.
- I identified Instagram feasibility, and which images Lydia prefers for the hero slideshow and About section, as the remaining open questions. Form location and privacy/data-handling details are still tracked as an implementation blocker in US05.

**Rejected**

- None recorded. The usability targets are goals and not mandatory acceptance criteria, as recorded above.

### Limits of this evidence

- The rough notes are the source evidence for the original draft.
- The two-working-day response target is my account of a conversation with Lydia and has no separate written record.
- The three screenshots show only parts of the conversation: my first request with the initial review (model GPT-6 Luna), the questions and my answers, and my later logging request with the completion summary. They show clock times only, not dates, so the date comes from my own record. The answers screenshot is cropped on the right.
- My clarifications about deposits and the two-working-day reply aim are not in any screenshot. They appear only in the conversation text.
- Copilot wrote this entry and `docs/brief.md`. I have not yet confirmed with my teacher that AI drafting is permitted for this assessment, and the JCQ declaration is still to be completed.
- This entry and the brief do not establish that Lydia has reviewed or signed off the new brief, that the proposed design has been built, or that the site has been tested.


## Entry 11: User-story review and sprint-plan alignment

**Date:** 8 November 2026  
**Tool:** Copilot Chat in VS Code  
**Reference:** GitHub (2026) *GitHub Copilot Chat* [Generative AI]. Available from: https://github.com/features/copilot [Accessed 8 November 2026].

**Purpose:** To review my user stories against the planned build and align the transition from Sprint 0 into Sprint 1 and later page-focused sprints.

**Authorship:** Copilot reviewed the documents, made recommendations, and drafted and applied wording to the planning documents after I approved its proposal. I provided the decisions and clarifications recorded below. Copilot also drafted this proposed log entry.

### Interaction record

| Step | My request or response | Copilot’s contribution |
|---|---|---|
| 1 | I asked for a review of my user stories against my planned build. | Copilot identified a difference between the brief and Sprint 1 scope and raised questions about priorities, reviews, the gallery, story statuses, the hero fallback and cancellation wording. It made no edits during this initial review. |
| 2 | I gave my decisions and asked to see the proposed update before any edits. | Copilot presented a proposed update in chat. |
| 3 | I approved the proposal as written for refactoring. | Copilot changed the brief, user stories, Sprint 0 carry-forward items and Sprint 1 plan. |
| 4 | I asked for a draft AI log and then asked for my decisions and rejected suggestions to be clearer. | Copilot revised its proposed log and distinguished my decisions from its recommendations. |

### Screenshots

- [Review request and initial findings](screenshots/story-review-summary.png): my request, Copilot's review and the beginning of my response.
- [My responses to the review](screenshots/story-review-decisions.png): my decisions and clarifications about the findings.
- [Approval and activity](screenshots/story-review-approval.png): my approval and Copilot's activity summary; the full proposed wording is not visible.
- [Update summary](screenshots/story-review-update.png): Copilot's summary of the planning-document changes.

### My decisions and responses to AI suggestions

#### Accepted or chosen

- **Sprint structure:** I chose smaller sprints, with a separate sprint for each page, to support testing and version control. The updated brief also includes a later integration, deployment and handover sprint.
- **Reviews:** I confirmed that I want a review carousel on the homepage and a separate full Reviews page. They are planned for different sprints.
- **Story status:** I clarified that “In Progress” includes research and planning already started. Implementation and test evidence will be added later.
- **Must priorities:** The updated plan says Must stories are required before public launch, but do not all need to be completed in Sprint 1.
- **Unfinished pages:** I said links should still work while page content is being built. I approved the proposed “Coming soon” placeholders. These do not count as completed pages or stories.
- **Enquiry location:** Lydia’s feedback mentions “their address” and separately states that her service area is Banbury and surrounding villages. Copilot suggested omitting the separate address field, incorrectly treating the service-area confirmation as support for that suggestion. I initially approved the proposal including that omission, then reconsidered, withdrew that approval and decided the form should require the client’s full address. The full-address requirement is my subsequent decision; Lydia's feedback does not separately confirm its scope or requiredness.
- **Privacy information:** I said privacy and data handling could be mentioned in the FAQ and footer. The approved update also makes the notice accessible from the form and keeps verification of the actual provider and data handling as a condition before live submissions.
- **Cancellation:** I said the notice had been confirmed as one day. 
Reconcile the address, reply-time and hero-fallback records.

#### Suggestions I did not adopt or clarified

- **Gallery default:** Copilot suggested a curated hand-built gallery as the default. I did not adopt that recommendation. Lydia controls the photos she publishes to Instagram, and I want to explore using those posts so she can control updates without involving me. A hand-built gallery remains the fallback if Instagram display is not technically practical.
- **Status evidence:** Copilot questioned whether the “In Progress” labels were supported by implementation evidence. I clarified that they also cover research and are not a claim that the features have been built or tested.
- **Client conversations:** I stated that I do not intend to record every conversation with Lydia.

#### Left unchanged or still to check

- **Review rotation:** Copilot suggested considering whether automatic rotation was worthwhile. I confirmed the carousel and separate page but did not explicitly reject auto-rotation in this exchange. The planned slow rotation and controls remained.
- **Hero fallback:** Copilot identified a mismatch between US01’s required slideshow and its static-image fallback. I edited the user story to clarify the intended feature and avoid an inaccurate claim.

### Documents changed after my approval

- [brief.md](brief.md): sprint sequence, gallery approach and enquiry details.
- [user-stories.md](user-stories.md): story-status and priority meanings, plus changes to US03, US04 and US05.
- [sprint-0.md](../sprints/sprint-0.md): enquiry-related status and carry-forward item.
- [sprint-1.md](../sprints/sprint-1.md): Home-page scope, placeholder behaviour, carousel checks and later page work.

Copilot reported that `git diff --check` passed. No tests were run for the documentation changes.

### limits of evidence

- The client clarifications above are my account in this conversation, not separate written records from Lydia.
- The screenshots cover only parts of the interaction; they do not capture the later address reconsideration. Its sequence is recorded from the conversation.
- This entry does not establish that the planned features have been built, tested or deployed.