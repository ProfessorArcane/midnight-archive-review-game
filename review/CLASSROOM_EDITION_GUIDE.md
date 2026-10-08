# The Midnight Archive | Classroom Edition

**Prepared:** October 8, 2026  
**Instructor:** Holguin / Professor Arcane  
**GitHub repository:** https://github.com/ProfessorArcane/midnight-archive-review-game  
**New classroom page in GitHub:** https://github.com/ProfessorArcane/midnight-archive-review-game/blob/main/classroom.html  
**Intended GitHub Pages route, if Pages is enabled for the repository:** https://professorarcane.github.io/midnight-archive-review-game/classroom.html  
**Offline backup:** `Midnight_Archive_Classroom_Ready_20261008.html` (all CSS, JavaScript, and questions included; no internet required when opened locally in a desktop browser).

## Class launch in 60 seconds

1. Open the **classroom.html** page on your classroom Mac/TV projector, or download/open the self-contained offline HTML file.
2. Choose a **Question pool** and **Board**, then choose **2, 3, or 4 teams**. Click into the team name fields to rename them.
3. Click a point tile to reveal the question and four neutral answer choices. Only the instructor controls **Reveal answer**.
4. Use the **15/30/45/60-second timer** as desired. After revealing, read the teaching explanation and any **Texas law note**. Award or subtract the tile's points using the team buttons, or close without points.
5. The used tile becomes unavailable. Use **Board** for another round. **Reset game** clears scores and tiles and starts a new session.

### Choosing the pool

| Pool | Contents | Good for |
|---|---|---|
| Recovered · exclude marked holds | 63 recovered questions without **identified** curriculum holds | General review from concepts already taught. Still check class readiness; not every prerequisite is detectable from text. |
| All recovered questions | 100 recovered source records, including material with teaching holds | Instructor-controlled review **after** relevant lessons. |
| PHRA 1009 · Weeks 1–2 math | 12 calculation/conversion questions selected from foundational topics; some are reconstructed | Focused math review after you confirm the relevant lessons were taught. |
| PHRA 1009 · All math lessons | 20 calculation items, including future topics | Later PHRA 1009 review only; **not** for introductory week. |
| All 210 · includes reconstructed drafts | 100 recovered + 110 newly reconstructed item texts | Instructor **editorial preview** until reconstructed wording is fully revalidated. Contains seven full 30-tile boards. |

**Do not mistake a previously approved topic/answer key for approval of new prose.** Q011–Q120 were rewritten from the instructor's approved topics and keys after the exact earlier question wording could not be recovered. They are explicitly labeled **RECONSTRUCTED** in the editorial master and classroom answer reveals.

## What changed, what did not

- This release adds **`classroom.html`** as a *separate page*. The existing live **`index.html` was not modified**.
- The classroom file is **standalone**, with data embedded rather than fetched separately, so it can run offline.
- The main board is six columns × five point tiles, with partial final boards when a question pool does not divide evenly into 30.
- Scores, team names, the selected pool/board, and used tiles are designed to persist in the same browser's local storage. Reset game deliberately clears score and tile progress.
- The correct answer and explanation appear **only after reveal**. Relevant national-versus-Texas rules appear in **after-answer notes** on Q110 and Q136.
- The explanation for Q190 uses both `C₁V₁ = C₂V₂` and `SC × SV = DC × DV`, the stocked/have versus desired/want setup, and **q.s. to 80 mL final volume**.

## Quality and responsible use

- **210/210** items have a unique numeric ID, a stem, four distinct options, an answer letter, and explanation. **No exact duplicate stems** in the 210-question editorial draft.
- Of 210, **100** preserve recovered source wording; **110** are reconstructions, not original approved full text.
- Browser tests exercised load, 30-tile board population, 2–4 teams, scoring, answer reveal, changing boards, timer controls, and mobile horizontal scrolling. The automated browser tests passed locally, but the **GitHub Pages served URL could not be reached from the inspection environment**, so public hosting must not be claimed independently verified.
- NHA ExCPT-style educational questions are not official NHA exam questions. This is a **review game**, not a blueprint-weighted scored practice examination. The official 2025 ExCPT blueprint has 15% roles, 15% laws, 13% drugs/therapy, 43% dispensing process, and 14% safety/QA: https://info.nhanow.com/hubfs/Test%20Plans/2023%20ExCPT%20Test%20Plan.pdf
- A final instructor curriculum crosswalk and independent fact check of reconstructed wording remains prudent **before enabling the all-210 mode for students**. Never assess content the learners have not been taught.

## Source/correction inventory

- Current instructor approval register: https://github.com/ProfessorArcane/midnight-archive-review-game/blob/main/review/INSTRUCTOR_APPROVAL_REGISTER.md
- Approval metadata: https://github.com/ProfessorArcane/midnight-archive-review-game/blob/main/review/QUESTION_METADATA_001_210.json
- Original 210 Gemini export is **not** the approved numbered bank. Source Q021–110 corresponds to approved IDs Q121–210, with all 90 matching their approved answer-letter assignments. Q001–010 recovered from original Batch01.
- For Q110, federal inventory is at least biennial while Texas generally imposes annual inventory for applicable pharmacy types. For Q136, qualifying initial-fill electronic transfers of Schedule II prescriptions are permitted if all legal requirements are met; C-II refills are still prohibited. State-law notes must be **after reveal** only.

## Publication notes

1. The standalone `classroom.html` was added to the **main** branch independently of the existing playable game.
2. The existing `index.html` remains untouched.
3. If the GitHub Pages URL does not open, open the offline HTML file immediately for class. Separately check Settings → Pages → source branch `main` and folder `/ (root)` in GitHub; this is an optional hosting setup step, not required for offline use.