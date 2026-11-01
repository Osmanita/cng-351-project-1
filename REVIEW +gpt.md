# Review of the corrected CNG 351 report

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
