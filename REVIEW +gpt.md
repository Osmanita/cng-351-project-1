# Review of the corrected CNG 351 report

## Current B1-B2 revision

The seven report-text pages use shorter sentences and simpler vocabulary. Necessary ER terminology, identifiers and all entity-key tables are retained. All three use cases were compared against the prior source: 6/7/8 rules, 4/4/5 assumptions, date and subset conditions, stored/derived values and uniqueness rules remain. Past employment wording was clarified to preserve former companies and rental history. The ongoing-rental definition explicitly requires both date conditions.

The cover and all eight full diagram pages, including their notes, have identical content streams to the previous PDF. All revised text pages were rendered and individually inspected. No clipped text, overlaps or broken tables were found. The report has 16 pages with the same dimensions, order and footers. No new external detector result is available.

SHA-256: `AAA10F485BB473C5D92614EEE8914210105389C6CCF4C894209CC0702C61ED13`.

## Prior revision

Current PDF: `CNG351_Assignment1.pdf`, 16 pages. Pages 2, 3, 4, 7 and 8 have revised explanations; page 6 has three revised notes. All eight diagram image payloads and placements are unchanged; the page 6 plotted region was compared pixel by pixel. The cover, UC3 and the other seven full diagram pages are unchanged. Key tables, 41 checked modelling conditions and all 67 technical identifiers are retained. Source XML differs only in UC1B text_2, text_3 and text_4. Revised pages were rendered and individually inspected; no clipping or overlaps were found. The new document has not been retested by an external AI detector.

SHA-256: `B9ECF21E81635E3E6104B593AE11D094F26C8C15366DFA02C490DF61D52660A0`.

## Earlier reviews

Current PDF: `CNG351_Assignment1.pdf` (16 pages). Its final language edit preserves 56 checked technical conditions, 67 technical identifiers, all key tables, the cover and all eight full diagram pages. The Requirements source paragraph on page 2 was subsequently removed; all other 15 page content streams remain unchanged by that removal. The changed text pages were visually reviewed. No QuillBot/GPTZero score has been obtained.

SHA-256: `6F55D981F161160EE19A98D115A6D3B7B6E35963CCA5E9ED478F7BB5A6B7FE76`.

The review below records the earlier technical repair.

All 24 findings from the external rewrite were repaired. The report was checked against the approved model, and all 16 pages were rendered for layout review. No remaining new content or layout issue was found in this review.

## Repairs

| Item | Page | Repair | Result |
|---|---:|---|---|
| 1 | 13 | Each Rental links one company to one office | PASS |
| 2 | 7 | UsageSession is weak under Machine | PASS |
| 3 | 8 | Machine.Type; Dormitory.Level; Student.Username; Student.Age | PASS |
| 4 | 8 | completed; completed or interrupted; scheduled or cancelled sessions may have no actual-use dormitory | PASS |
| 5 | 10 | Student.Username is unique in addition to StudentID. | PASS |
| 6 | 14 | Represents is a subset of WorksFor. | PASS |
| 7 | 13 | EmploymentStartDate is an attribute of WorksFor. | PASS |
| 8 | 13 | Each company has one representative; an employee represents at most one company. | PASS |
| 9 | 13 | active; ActualSubmissionDate may be NULL until submission. | PASS |
| 10 | 13 | The supervisor must WorksFor the same company as the intern. | PASS |
| 11 | 13 | The ongoing-rental rule applies only to companies currently operating in the building. | PASS |
| 12 | 8 | Stay periods for one student must not overlap. | PASS |
| 13 | 4 | Each question has question text and belongs to at least one category. | PASS |
| 14 | 8 | EndTime may be unknown for unfinished/cancelled sessions; duration needs both time bounds. | PASS |
| 15 | 11 | UsageSession is identified by (MachineID, SessionNo). | PASS |
| 16 | 6 | IsCorrect is stored and checked by comparing answers. | PASS |
| 17 | 12 | EmployeeCount* is stored and refreshed automatically whenever current WorksFor links change. | PASS |
| 18 | 13 | A company may rent the same office again under a new RentalID. | PASS |
| 19 | 2 | Preserve the original symbol/meaning rows. | PASS |
| 20 | 4 | Separate assumption paragraphs. | PASS |
| 21 | 8 | Separate assumption paragraphs. | PASS |
| 22 | 13 | Separate assumption paragraphs. | PASS |
| 23 | 5 | Consistent readable note font; input uses 9.48 pt. | PASS |
| 24 | 16 | Consistent readable note font; input uses 9.48 pt. | PASS |

## Final checks

- 16 pages, with the supplied A4 portrait and A3 landscape page sizes and the same page order.
- Cover content and rendered appearance are identical, including Group 8 and both student IDs.
- The eight diagram image payloads, placements and rendered diagram regions are identical to the uploaded PDF. Labels, keys, connector lines and cardinalities are preserved.
- Entity/key tables match the input after whitespace normalization.
- Business rules and assumptions are complete, including the stored IsCorrect rule, independent username uniqueness, nullable use-dormitory cases, date boundaries, historical records and same-company supervisor rule.
- All four UC1 and UC2 assumptions and all five UC3 assumptions are separate paragraphs.
- Legend is a two-column table. Main prose and drawing notes use 11.5 pt text; no note-font shrinking.
- Correct x of 16 footers on pages 2-16, none on the cover. No form fields or widgets.
- No text extends beyond the page bounds. All seven body-text pages were inspected individually; all note text and the eight-diagram contact sheet were inspected.
- The editable draw.io model, coordinates, connector styles and partial-key marks are unchanged. Only the 21 note texts were updated to match the report.
- Earlier decisions are retained: repeated questions and repeated joker types are allowed; IsCorrect remains stored; no new booking-overlap rule was added.
- The rental interval assumption now explicitly calls a NULL EndDate open-ended. Whether the rental is ongoing still depends on both StartDate and EndDate, as the approved rule requires.

## Existing format limitation

The uploaded input already contains raster diagram images rather than vector PDF drawings. Those images were preserved exactly, so the corrected PDF retains that format. The editable draw.io file is available for later vector export. The legend no longer incorrectly describes the PDF drawing pages as vector.

## Files

- Current report: CNG351_Assignment1_Report +gpt.pdf in the repository.
- Matching editable source: CNG351_Assignment1_Chen +gpt.drawio in the repository.
- Local output: CNG351_Assignment1_Report +reviewed.pdf.
- PDF SHA-256: c440913c0a3e00f99941ccbdd8702afa05678b48f4f4636197f5b45d6cbb3f7c

## Follow-up clarification on page 3

Before: These binary links allow up to four joker uses without a ternary relationship.

After: These links avoid a ternary relationship; the limit of four joker uses comes from Contestant's (0,4) participation in HasJokerUse.

The (0,4) was checked against Contestant in HasJokerUse in the editable source. All other 15 page content streams, all eight diagram images, page sizes and footers are unchanged.
