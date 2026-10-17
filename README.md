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
- **Enquiry form**: validates the visitor's details and sends them to
  vincdeeptech@gmail.com through [FormSubmit](https://formsubmit.co). If the
  send fails, the visitor can email or copy the request instead.

## Motion

- **Background**: a slow network of nodes in the four VINC colours drifts behind
  the page like a circuit, shifts as you scroll and reaches toward the pointer.
  Soft colour glows move behind the hero, and its grid drifts.
- **Foreground**: the hero's four parts fly in and snap together, then float and
  tilt toward the pointer; "build" gets a hand-drawn underline. Meshing gears turn
  as you scroll, a ticker of programme topics runs between sections, cards glow
  under the pointer, and a four-colour bar under the header shows scroll progress.
- **On scroll**: sections lift in, the 100 seats fill one by one, struck-through
  words draw their line, and panels ease in when a tab or day changes.

Everything is readable at rest, and visitors who set "reduce motion" on their
device get a still page.

## Before going live

- **Activate the enquiry inbox**: the first enquiry sent from the live site makes
  FormSubmit email vincdeeptech@gmail.com an activation link. Click it once, and
  every later enquiry arrives as an email. FormSubmit then offers a random alias
  you can put in `LEADS_INBOX` (top of the script in `index.html`) so the Gmail
  address no longer appears in the page source.
- **Policies**: each page in `policies/` says the policy is being finalised.
  Replace that text with the approved policy wording.

## Preview locally

```sh
python3 -m http.server 8000
# then open http://localhost:8000
```
