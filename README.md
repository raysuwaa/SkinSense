# SkinSense

AI skincare assistant website built for BIS 310 Introduction to Software Engineering (Umm Al Quwain University, Dr Hanan Hussain, 2026-2027).

Team: Raghd Qaid (24121061), Dina Eid (25124076)

## What it does
1. The user answers questions about skin type, concerns, allergies, pregnancy, age and habits.
2. The user adds a photo (upload or camera) or continues with answers only.
3. An AI model returns findings with severity and confidence, a barrier check, a morning, evening and weekly routine, a product guide, an avoid list, habit advice and a timeline.
4. A rule engine in code hides catalog products that conflict with allergies, pregnancy or age, and shows the reason.

SkinSense is educational and is not a medical diagnosis.

## Roles
- **User:** signs in, runs analyses, searches and deletes their own history.
- **Administrator (owner/editor):** manages the product catalog (create, view, update, search, delete) and sees the usage report.
- Sign-in is handled by the viewer's Claude account; the app stores no passwords.

## Database
Collections: `products` (catalog), `usage` (one document per user with run records), `data/users/<id>` (private saved reports; photos are never stored).

## Run
Open the published page and sign in. File: `skinsense.html` (single self-contained HTML page).

## Tests
See Section 9 of the final report.

## AI use
Generative AI (Claude) helped write the code and draft the report. The team reviewed and tested the result.

## Limits
Claude-account sign-in; 16 generic catalog products; no delete-account button; not tested on dark skin tones.
