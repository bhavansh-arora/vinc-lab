# VINC Bengaluru North

Website for the **VINC Learning Centre for Skill Education, Bengaluru North**,
built from the VINC business-plan and Centre 1 go-to-market decks. It covers
one centre only. Financials, the expansion plan and the founder profile are
deliberately left out.

A single static page with no build step: `index.html` holds the HTML, CSS and
script; `assets/` holds the logo in light and dark versions.

## Interactive parts

- **The sum of parts**: tap Build, Code, Explore or Careers in the hero.
- **Programme finder**: pick a grade (6–12) to highlight Building or Applied AI.
- **A week at the centre**: opens on today's day. Weekdays show undergraduate
  courses and school work, weekends show the Grades 6–12 batches.
- **Seat board**: 100 weekend seats in four batches of 25.
- **Free start**: a four-step walkthrough (sign up, skill score, demo class, enrol).
- **Who the centre serves**: tabs for parents, schools, teachers and undergraduates.
- **Opening plan**: marks the current and next week from today's date.
- **Enquiry form**: validates the visitor's details and builds a request they can copy.

## Before going live

- **Contact details**: fill in `CENTRE` (address, phone, email) at the top of the
  script in `index.html`. Until then the page shows bracketed placeholders.
- **Enquiry form**: it prepares a request for the visitor to copy. To collect
  requests directly, point the submit handler at a form service or CRM webhook.
- **Opening dates**: the timeline uses the planned 19 Oct – 29 Nov 2026 sprint
  dates. Edit the `data-start` / `data-end` values if they change.

## Preview locally

```sh
python3 -m http.server 8000
# then open http://localhost:8000
```
