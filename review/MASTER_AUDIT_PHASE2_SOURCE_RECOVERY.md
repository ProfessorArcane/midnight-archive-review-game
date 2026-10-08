# The Midnight Archive — Phase 2: Source Recovery and Metadata QA

**As of 2026-10-08**  
**Status:** Source audit and ALL 210 question-ID metadata index complete. **Word-for-word QA remains blocked for Q011–Q170.**  
**Working index:** `review/QUESTION_METADATA_001_210.json` (NOT a question-bank import file)  
**Live `index.html`: untouched.**

## What was found

Search of the October 8 Library uploads, the current GitHub repository (`index.html`, `content/` and `review/`), and prior-conversation indexed materials found:
- Q001–Q010: Complete original stems, 4 choices, proposed keys and rationales available in Library file `Midnight_Archive_ExCPT_Gemini_Review_Batch_01.md` (also .txt). Can import once matching corrections in approval register.
- Q011–Q160: Fifteen Gemini audit uploads and approval register cover names, topics, keys and corrections, but the accessible materials **do not preserve all exact original question stems, four exact choices or original revealed explanations**. Searches for Batch02 full question text specifically returned audit summaries, not the original assistant-authored items.
- Q161–Q170: A condensed prior-conversation summary plus reviewed answer keys is available, but **not the exact complete original ten questions verbatim**. Treat as missing original full text.
- Q171–Q210: The final 40 questions' complete original batch messages are visible in the current conversation, but no consolidated canonical GitHub file has yet been committed. Preserve exact wording rather than replacing it with review-table paraphrases.
- The 31 legacy playable live questions and a separate Final are in the encoded live `index.html`. These are NOT the same as the newly reviewed 210-question MC bank.

## Integrity checks completed on derived 210-item metadata

| Check | Result |
|---|---|
| Expected ten batches ×? | **21 batches × 10 = 210 IDs** |
| Unique sequential question IDs | **210 / 210; Q001 through Q210** |
| Recorded proposed correct answer letters | **210 / 210** |
| Answer-key distribution | **A: 47, B: 58, C: 60, D: 45** |
| Original full text independently recoverable in Library | **10 items, Q001–Q010** |
| Missing original wording and all four exact answer options | **160 items, Q011–Q170** |
| Full original wording visible in recent chat but not yet canonical | **40 items, Q171–Q210** |
| Per-question NHA codes missing specifically from table fields | **20 Qs, Q001–Q010 and Q021–Q030**; their approval prose / original draft has some code references. **Do not interpret null table field as content gap in NHA coverage.** |
| User-approved answers in bank | **210** |
| Live `index.html` changes | **0** |

### High-priority thematic redundancy / comparison pairs

These are **topic-level potential overlaps**, not a verified word-for-word duplicate finding:

1. **Q089 + Q169: MEDICATION RECONCILIATION**. Both metadata summaries state technician collects/compares lists and reports discrepancies to pharmacist. This is the **strongest candidate for near-duplicate concept/answer**, requiring the precise original stems and options, then either change or defend one after instructor preview. Retain both approvals until a decision.
2. **Q088 + Q165: NCC MERP Category B vs C**: preserve if clearly different error-harm scenarios and teaching is complete.
3. **Q060 + Q155 + Q205: Class I/II/III recalls**: purposeful scaffold, distribute across boards.
4. **Q029 + Q195: pseudoephedrine CMEA**: confirm retail control vs 3.6g daily limit are different competencies.
5. **Q008 + Q160: markup**: one finds markup percent from cost/sale, other selling price from markup on cost; preserve if students have met K.122 in PHRA1009 Meeting8.
6. **Q036 + Q097**: oral-liquid days supply vs volume needed for dose course; verify distinct arithmetic demands.
7. **Q024 + Q196**: otic/ophthalmic interpretation; Q196's 2 gtts AU BID applies language safety and must be written out on label.
8. **Q027 + Q106 + Q167**: Orange Book, Purple Book and ASHP injectable compatibility reference, intentionally different reference types.
9. **Q057? vs Q158**: Q057 is missing patient name, **NOT** BIN; correction to a preliminary example grouping. Actual BIN/PCN overlap is **Q058 and Q158**.
10. **Q015 and Q016**: both brand–generic recognition but different ingredients/uses, not a sufficient reason to remove.
11. **Q061 and Q100**: spironolactone class versus OTC potassium supplement interaction, distinct skills.
12. **Q018 and Q053**: both ethinyl estradiol combination contraceptives but distinct hormone components and brands, hold until reproductive instruction.

**Reconstruction rule:** Any freshly reworded question in place of an unrecoverable original must be labeled **RECONSTRUCTED / NEEDS REAUDIT / NOT ORIGINAL APPROVED WORDING** until instructor explicitly reapproves it. It would be misleading to claim the 210 are one complete, directly playable validated corpus based solely on approval metadata.

## Preliminary code emphasis from INCOMPLETE review table cells

In the metadata index (which contains code strings for 190 items, but Q001–010 and Q021–030 lack the table-based code field), the most common codes are:
- **K.68 brand/generic: 64** annotated items;
- **K.61 indication: 59**;
- **K.57 therapeutic classes: 57**;
- **K.59 dosage forms: 17**;
- **K.62 body systems/disease states: 13**.

**Important:** Multi-code overlaps and empty table fields make these counts unsuitable as primary-domain NHA blueprint coverage. The final normalized bank needs exactly one *primary domain* per item, separate secondary K-tags, and a computed distribution against the official ExCPT **15% role/general duties, 15% law, 13% drug therapy, 43% dispensing processes, 14% safety/QA**.

## Next practical gates

1. **Recover exact old batch messages** Q011–Q160 from original October 8 conversation history (copy those 15 batch posts, or supply a selective exported chat transcript). Keep original stem and all four answer choices; do not use Gemini's answer/distractor paraphrases as substitute wording.
2. Copy original exact Q171–Q210 from recent conversation into draft-only structured JSON, preserving approval provenance, while the source is still visible. Q161–Q170 need source recovery alongside Q11–Q160.
3. Compare every new structured item with instructor corrections in the register; use verified source URLs, teaching holds and post-answer-only Texas notes.
4. Run actual **word-for-word duplicate detection, option/key schema validation, item coverage and board sequencing** on the canonical 210 items; submit suggested replacements for separate approval.
5. Assign six 30-question weekly boards and one 30-question championship board; keep FINAL separate, game untouched until explicit publishing instruction.

This report is a documentary *recovery* and metadata audit, **not completion of the full 210-question content audit**.
