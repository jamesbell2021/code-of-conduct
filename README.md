# Student Code of Conduct — induction guide

A single-page, self-contained web app that walks students through the Belfast Met **Student Code of Conduct** in plain English, checks understanding with a short quiz, and lets them sign, download and email a declaration confirming they've read and agree to it.

Live at: https://jamesbell2021.github.io/code-of-conduct/

## What it does

- Summarises the Code's purpose, the "Learning the Met Way" (CARE) values, students' specific obligations, and all ten categories of misconduct, in plain language.
- A short multiple-choice quiz to check understanding before signing.
- A declaration form: name, email, course, campus, a choice of lecturer to send it to, three tick-box confirmations, and a draw-your-own signature pad.
- **Download** — generates a self-contained HTML file of the signed declaration for the student's own records.
- **Print / Save as PDF** — opens the browser print dialog on a clean, print-only version of the declaration.
- **Email** — opens the student's own email client, pre-addressed to whichever lecturer the student picked from the dropdown, with the declaration details filled in. Browsers can't attach files to an email automatically, so students are prompted to attach their downloaded copy before sending.

### Lecturers students can send to

Edit the `LECTURERS` array near the top of the `<script>` block in `index.html` to add, remove or rename recipients:

```js
var LECTURERS=[
 {name:"James Bell",email:"jbell@belfastmet.ac.uk"},
 {name:"Phil Roddy",email:"proddy@belfastmet.ac.uk"},
 {name:"Anna Owens",email:"AOwens@belfastmet.ac.uk"}
];
```

## Important

This page is a **summary for learning purposes**, not the policy itself. The binding document is Belfast Met's own published [Student Code of Conduct (PDF)](https://www.belfastmet.ac.uk/media/ub0nm4j3/student-code-of-conduct.pdf) — where the two differ, that PDF is what counts. The summary here is based on policy version 10.0 (reviewed 02/07/2026); re-check against the source PDF if the College publishes an update.

## Tech

Plain HTML/CSS/JS, no build step, no dependencies, no backend. Nothing typed or drawn on the page is sent or stored anywhere except the student's own downloaded file and, if they choose to send it, their own email. Matches the visual theme of the [Day One induction guide](https://github.com/jamesbell2021/web).

## Running locally

Just open `index.html` in a browser, or serve the folder with any static file server.
