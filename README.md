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
- **Seat picker**: pick a batch, then a seat in its 25-seat cabin (five rows,
  an aisle), like choosing a seat on a flight. "Request this seat" fills the
  enquiry form with the programme, batch and seat.
- **Free start**: a four-step walkthrough (sign up, skill score, demo class, enrol).
- **Who the centre serves**: tabs for parents, schools, teachers and undergraduates.
- **Enquiry form**: validates the visitor's details and sends them to
  vincdeeptech@gmail.com through [FormSubmit](https://formsubmit.co). If the
  send fails, the visitor can email or copy the request instead.

## Motion

- **Hero**: a slow network of nodes in the four VINC colours drifts behind the
  opening section like a circuit and reaches toward the pointer, with soft colour
  glows and a drifting grid. The four parts fly in, snap together, float and tilt
  toward the pointer; "build" gets a hand-drawn underline.
- **Section companions**: a robot arm takes blocks off a conveyor and stacks four
  of them (Why now), a three-gear train turns all the time and faster as you
  scroll (Programmes; two gears in Start for free), a demo-day scene shows a
  student pitching a startup (GreenBin, an AI waste-sorting bin) at a lectern while
  the slides change and three judges raise score cards (How a quarter works), a rover drives along its
  lane (The week), signals run along circuit traces into a chip (Who the centre
  serves), a drone hovers with a question parcel (FAQ) and a paper plane loops
  beside the contact details. The larger pieces hide on narrow screens.
- **Elsewhere**: a topic ticker, pointer glow on cards, a four-colour scroll
  progress bar, sections that lift in on scroll, seats that pop in, and panels
  that ease in when a tab or day changes.

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
