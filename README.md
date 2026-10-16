# VINC Bengaluru

Website for the **VINC Learning Centre for Skill Education, Bengaluru**,
built from the VINC business-plan and Centre 1 go-to-market decks. It covers
one centre only. Financials, the expansion plan and the founder profile are
deliberately left out.

A static site with no build step: `index.html` holds the HTML, CSS and script;
`assets/` holds the logo in light and dark versions; `policies/` holds the six
company policy pages linked from the footer.

## Interactive parts

- **The sum of parts**: tap Build, Code, Explore or Careers in the hero.
- **Programme finder**: pick a grade (6–12) to highlight Building or Applied AI.
- **A week at the centre**: opens on today's day. Weekdays show undergraduate
  courses and school work, weekends show the Grades 6–12 batches.
- **Seat board**: 100 weekend seats in four batches of 25.
- **Free start**: a four-step walkthrough (sign up, skill score, demo class, enrol).
- **Who the centre serves**: tabs for parents, schools, teachers and undergraduates.
- **Opening plan**: marks the current and next week from today's date.
- **Enquiry form**: validates the visitor's details and builds a request they can
  copy or open in their email app, addressed to info@vinc-lab.com.

## Motion

The hero's four parts fly in and snap together, the grid drifts and "build" gets
a hand-drawn underline. Below the fold, sections lift in as they scroll into view,
the 100 seats fill one by one, struck-through words draw their line, and panels
ease in when a tab or day changes. Everything is readable at rest, and visitors
who set "reduce motion" on their device get a still page.

## Before going live

- **Phone number**: fill in `CENTRE.phone` at the top of the script in
  `index.html`. Until then the page shows a bracketed placeholder.
- **Policies**: each page in `policies/` says the policy is being finalised.
  Replace that text with the approved policy wording.
- **Enquiry form**: it prepares a request for the visitor to copy. To collect
  requests directly, point the submit handler at a form service or CRM webhook.
- **Opening dates**: the timeline uses the planned 19 Oct – 29 Nov 2026 sprint
  dates. Edit the `data-start` / `data-end` values if they change.

## Preview locally

```sh
python3 -m http.server 8000
# then open http://localhost:8000
```
