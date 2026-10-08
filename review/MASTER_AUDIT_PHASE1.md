# The Midnight Archive — Master Audit, Phase 1

**Audit date:** 2026-10-08  
**Status:** Structural and documentary audit completed; **NOT ready to publish**.  
**Source of truth:** `review/INSTRUCTOR_APPROVAL_REGISTER.md` (21 ten-question instructor approvals, Q001–Q210); existing `index.html`; four separate draft content JSON sources and instructional notes; NHA's official ExCPT plan linked below.  
**Invariant:** **Do not change live `index.html`, existing questions, or gameplay without separately explicit instructor authorization.**

## Executive finding

- **210/210 reviewed question IDs are instructor-approved**, subject to mandatory recorded answer-explanation, NHA-code, teaching-hold and Texas-note corrections. This is an approval *register*, not a finished question-bank file or deployment authorization.
- **All 21 batch headings now show Approved.** Batch16 mistakenly retained a 'pending' heading despite instructor approval during the conversation. The approval register was reconciled on 2026-10-08 without changing answers or the playable game.
- **Blocking publication gap:** The GitHub repo does **not yet contain one complete canonical structured file of all 210 stems, four answer choices, marked correct letters, explanations, NHA codes and teaching holds**. The register predominantly stores **short topic summaries and corrections**, not the full exact question text. The approved 210 cannot be truthfully described as having completed a full *word-for-word* duplicate audit or as ready for import until that source file is assembled from the original instructor-approved question batches and checked against this register. Do **not** silently reconstruct approved wording from topic summaries and call it identical.
- The current **live** game has **31 legacy questions + one separate `FINAL`**. Live category counts: **Sig Decoder 5; Pharmacy Workflow 6; Stem Detective 5; Medication Match 5; Insurance & Law 5; Patient Safety 5**. Pharmacy Workflow has two 400-point slots, resulting in 31 rather than 30. Existing live activities include **Individual, Board Race, Team Discussion**, largely free-response, while new bank questions are four-choice MC. This creates a **game-engine and mapping design task** even after question-bank assembly.
- Independent draft-only files exist under `content/`, and **must NOT be conflated with these 210 approved MC questions**:
  - `draft_excpt_reproductive_questions.json`: 12 ExCPT-style drafts + 10 reproductive drafts;
  - `draft_body_systems_excpt_questions.json`: 36 draft items;
  - `body_system_excpt_extension_draft.json`: 30 draft weekly + 8 supplemental;
  - `draft_student_photo_excpt_expansion.json`: 23 draft items;
  - Combined raw draft entries = **119**, with potentially overlapping subjects and no guarantee of approval or distinctness. These are *not* additional 119 approved questions.

## Current official NHA ExCPT blueprint

NHA's current ExCPT exam version launched **July 9, 2025**; its publicly linked test plan is titled **2023 ExCPT Test Plan** because it is **based on a 2023 job analysis**, not because it expired in 2023. NHA's official update announcement confirms applicability for exams on/after July 9, 2025:
- https://info.nhanow.com/mediacenter/coming-soon-new-excpt-certification-exam-study-materials
- https://knowledge.nhanow.com/hubfs/Test%20Plans/2023%20ExCPT%20Test%20Plan.pdf

Current **100 scored-item** domain weights:
| Domain | Official scored items | Percent |
|---|---:|---:|
| 1. Role, Responsibilities, General Duties | 15 | 15% |
| 2. Laws | 15 | 15% |
| 3. Drugs and Drug Therapy | 13 | 13% |
| 4. Dispensing Process | 43 | 43% |
| 5. Medication and Patient Safety / QA | 14 | 14% |

**Audit action:** After canonical export, assign every item **one primary domain** (plus secondary tags as applicable). Count domain distribution on **each** board and across all 210. Distinguish weekly instructional reviews from a certification-simulation blueprint: weekly boards should follow what has been taught, whereas the championship should cover all five domains with attention to high-weight dispensing. Do not infer true blueprint coverage simply from multiple K-codes per medication-recognition question. Historical pharmacy laws are still covered, but NHA says the updated exam gives them *less emphasis* than previously.

## Topic overlap candidates requiring full-stem comparison

These are **potential clusters**, *not findings of verbatim duplicates*, because original full question wording for all 210 is not present together:

| Candidate items | Overlap and decision gate |
|---|---|
| **Q89 and Q169** | Both concern technician assistance with **medication reconciliation**. Compare question stem/answer logic; replace or revise one if both essentially ask "technician gathers and reports discrepancies". |
| **Q88 and Q165** | NCC MERP **Category B versus Category C**; should remain as deliberate progression *if* clearly distinct patient-reach scenarios and taught first. |
| **Q60, Q155, Q205** | FDA recall **Classes I, II, III**; progression, not duplication if each case is unique. |
| **Q55 and Q178** | DSCSA **suspect-product quarantine versus product identifier**; distinct objectives, keep if clear. |
| **Q27, Q106, Q167** | Orange Book, Purple Book, ASHP Injectable Drug Information; complementary drug-reference literacy, but avoid too many identical "choose a reference" stems on a single board. |
| **Q57/Q158 and Q22–23 in legacy live board** | BIN/PCN and insurance routing; complementary but may be repetitive if a board places them adjacent. |
| **Q8 and Q160** | **Markup**: percent from cost/selling price versus selling price from cost/markup percent; complementary calculations but should be separated by review/skill progression. |
| **Q29/Q195** | Pseudoephedrine behind-the-counter federal restrictions versus numeric daily 3.6g CMEA limit; verify each has a different learning target. |
| **Q24 and Q196** | Eye/ear abbreviation recognition, including AU vs OU; useful progression, but use unambiguous safe patient-label wording. |
| **Q31/Q47/Q136/Q179** | Controlled substance refill/transfer/emergency process; scope distinct if stems preserve legally different actions. |
| **Q97/Q170/Q139 and existing legacy days-supply questions** | Multiple days-supply applications; check uniqueness, level and sequencing rather than blanket removal. |
| **Q40/Q171/Q201** | Lipid medicines atorvastatin, ezetimibe, rosuvastatin; different drugs/classes except atorvastatin and rosuvastatin are both statins. Compare cognitive target and distribution across boards. |

## Preliminary course-placement controls (NOT finalized week assignment)

**Never assess before taught.** Pending a question-by-question crosswalk to final PHRA1001 six-week lessons, keep these *minimum* holds:

- **Reproductive products** including Q5, Q18, Q53, Q65, Q95, and comparable items: requires reproductive mini-lesson or documented prior instruction.
- **Neurologic/CNS recognition** including Q15, Q72, Q105, Q151, Q172, Q183, Q202: only after neurologic/CNS content taught; no arbitrary assumption all were taught in early PHRA1001 weeks.
- **Genitourinary** Q152, Q163, Q203 and other GU items: only after GU medication overview.
- **Safety/hospital/compounding** includes Q59, Q78, Q120, Q126, Q135, Q147, Q159, Q165, Q168, Q199, Q206: only after the respective nonsterile, sterile, high-alert, medication-error or bloodborne-pathogen lessons. Specific preparation tech may be better for PHRA1043 review rather than introductory weekly boards.
- **Drug information references** Q27, Q106, Q167: after reference literacy; **vaccines** Q134/Q204 after vaccine instruction.
- **PHRA1009 protected objectives** should follow this instructor's locked eight-meeting map:
  - Meeting **1**: temperature scales K.121 (e.g., Q180); other conversion/day-supply topics only after covered.
  - Meeting **3**: ratio strength K.116 (e.g., Q200), percent concentration K.117 (e.g., Q56), with exact part-in-total rule.
  - Meeting **4**: dilution/concentration K.118 (e.g., Q190). Worked feedback MUST show BOTH **`C₁V₁=C₂V₂`** and **`SC×SV=DC×DV`**, STOCK/HAVE vs DESIRED/WANT, **`SV=(DC×DV)/SC`**; optional classroom diluent = **`DV−SV`** only with additive-volume assumption; true compounding **q.s. to final volume**.
  - Meeting **5**: alligation K.120 (e.g., Q130).
  - Meeting **6**: safe-dose checks using **given** safe range K.144 (e.g., Q150).
  - Meeting **7**: IV flow rates K.119 (e.g., Q117, Q210), **mL/hr and gtt/min clearly distinguished**.
  - Meeting **8**: business math K.122 including markup (e.g., Q8, Q160).
  - **Other math** (mEq, days' supply, packaging, temperature, conversions) only after the actual PHRA1009 lesson in which each is taught. Do not blindly apply an external AI's incomplete "all math to PHRA1009" list.
- Week-specific distribution **cannot be finalized** from the register alone. Need the definitive lesson sequence and full source text for each question; PHRA1009 and PHRA1043 content must not leak into PHRA1001 early boards.

## Board and game integration plan (proposal, not a completed mapping)

**Instructor-approved target:** **6 weekly boards × 30 items** (=180) plus **one championship board × 30** (=210), plus a **separate Final**. A ten-question batch is an **auditing unit**, not a week. Do not infer Batch01=Week01.

For each of the **seven 30-cell boards**, select 6 categories × 5 difficulty/point levels, or another explicit instructor-approved arrangement. Track:
- Unique question IDs exactly once (unless user explicitly approves intentional retrieval repeats).
- Four answer choices and approved letter; **no bolded/visually premarked correct choice** in student-facing choices.
- Hidden answer feedback until reveal; Texas-only notes appear **only after answer reveal**.
- Instructor controls for assigning point values and teams; preserve original four-team game personality, live styles, scoring and existing questions until asked to change them.
- Separate `FINAL` remains outside 210-question tally, with the original final protected until instructor authorizes a new one.

**Presentation mismatch requiring design approval:** Legacy live board uses free-response/board race/team discussion; new 210 bank uses A/B/C/D. Decide whether weekly boards offer selected **MC-only** play, instructor-led reveals with physical whiteboards, or support both modes. Do not silently remove successful existing game behaviors.

## Required remaining phases and gates

1. **Collect canonical exact question text** Q001–Q210 from original reviewed batches and source chats/files: ID, title, stem, options A–D, correct letter, instructor-facing worked feedback, primary + secondary NHA code/task, authoritative source, teaching prerequisite/hold, federal vs Texas law note, status, batch audit provenance. Migrate corrections from approval register. *Do not generate invented text to fill a missing source and label it approved.*
2. **Automated and manual bank QA:** enforce 210 unique IDs and 840 answer options; verify exactly four choices and one key each; check near-duplicate stems, mathematically identical skills, repeated distractors, answer-letter distribution, term consistency and obsolete NHA descriptions.
3. **Curriculum crosswalk:** assign PHRA1001 taught-week versus PHRA1009/1043 content, with holds; verify against actual slides/Canvas teaching sequence before weekly assignment.
4. **Domain coverage and difficulty:** tally primary-domain distribution against NHA's current 15/15/13/43/14 scored distribution, while retaining educational reasons for any intentional differences; spot under-tested dispensing skills.
5. **Construct seven 30-cell boards** plus separate Final and propose student-facing reveal workflows. Check no board exposes answers, Texas note or future skills prematurely.
6. **Instructor preview and final sign-off.** After separate explicit deployment authorization, implement in the live game and perform gameplay regression tests. Until then **no index.html edits**.

## Progress and limitations

**Completed in Phase 1:** official source/version verification, repository inventory, legacy game count/category architecture, 21 approval-heading reconciliation, identification of structural publication blockers, preliminary duplicate/hold watchlist and board plan.  
**NOT completed:** canonical 210-question extraction, exhaustive duplicate/distractor/choice testing, all-question primary domain tally, final week assignment, MC implementation and gameplay test.  
**Status:** **NOT READY FOR LIVE PUBLICATION.**
