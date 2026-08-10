# Fast Track Farming — CRO Action Plan

Source: *Conversion Rate Optimization Review*, Pathmark Partners, Aug 4 2026.
Condensed into work items against the current `index.html`. Work top to bottom.

**Context:** Aug 16 bonus deadline is 6 days out. Ship the high-confidence fixes now; don't wait on A/B tests.

---

## Tier 1 — Ship first (trust + price)

### 1. Price says "+ HST" everywhere
Checkout charges $1,130; the page says $1,000. Fix every reference.
- Hero pill `💵 $1,000 per seat` → `$1,000 + HST`
- "Who This Is For" close: *"invest $1,000"* → `$1,000 + HST`
- Register section price anchor: `Ticket: $1,000`, `you pay $1,000`
- "After August 16" card: `Same $1,000 — $3,000 less value`
- Add `$1,000 + HST` next to every Reserve My Seat button

### 2. Reframe the 6% language
Disclaimer says no rate is guaranteed while the body promises 6% every time. That tension costs trust.
- Curriculum step 12: `Commission: Get 6% Every Time` → **Presenting Your Value & Holding Your Fee**
- "You want to hold your commission" card: drop *"so you sign at 6% every time"* → *"so you can present your value and hold your fee"*
- Hero lead: *"signing every listing at 6%"* → *"presenting your value and holding your fee"*
- Final CTA: *"sign at 6% every time"* → same reframe
- Keep the footnote/disclaimer as is

### 3. Rewrite the hero around the outcome
Currently the H1 is just the event name. Target structure:
- Eyebrow: `IN-PERSON WORKSHOP FOR GTA REALTORS®`
- H1: **Build Your Complete Geographic Farming Plan in One Day**
- Sub: leave with a defined farm, a written 12-step plan, door-knocking scripts, a marketing calendar and the systems to start immediately
- Line: `Tuesday, September 22, 2026 · 10:00 AM – 6:00 PM` / `Venu Event Space, Vaughan · $1,000 + HST`
- CTA: `REGISTER FOR SEPTEMBER 22`
- Reassurance line: in person with Monica · written materials included · early-registration bonuses until Aug 16
- Keep "Fast Track Farming" as branding above/below the H1, not as the H1

### 4. Credibility strip directly under the hero
Move a compact version of the About stats up: `10+ yrs #1 in Etobicoke` · `1,700+ homes sold` · `$1B+ volume` · `Top 0.1% of TRREB`. Follow it with **one** strong testimonial (name, brokerage, photo, specific result) — Renee Proulx's $1M is the strongest.

### 5. Add the venue address + event details
Page says only "Venu Event Space." Add full street address, city, parking note, lunch/refreshments, what's included, what to bring.

---

## Tier 2 — Structure and content

### 6. Add a one-day agenda
12 topics are listed but no shape for 8 hours. Add a timed agenda: farm plan → area selection → brand & marketing calendar → door-knocking demos → tracking → follow-up → open houses → fee conversation → 30-day implementation plan. Include breaks and lunch.

### 7. Reorder + shorten the page
Page is ~11,000px and repeats "own a neighbourhood," "hold your commission," Monica's experience, "complete system." Target sequence:
1. Outcome hero
2. Credibility strip
3. One powerful testimonial / video
4. What you'll leave with
5. One-day agenda
6. Who this is for
7. Monica's bio (shortened, tied to *teaching* farming)
8. Registration package + bonuses
9. Three detailed testimonials / case studies
10. FAQ
11. Final registration

### 8. Upgrade the social proof
- Move the YouTube testimonial video near the top
- Build 3 short case studies: what they implemented, how long farming, measurable result, photo, brokerage, farm area
- The 21-name "Happy Farming Students" grid is weaker than 3 detailed stories — shrink it

### 9. Make the bonuses credible
- Lead with what the private door-knocking session and post-event Zoom actually do for the attendee
- Keep `$1,500 / $1,500 / $3,000 / $4,000 total value` **only** if those are genuinely sold separately at those prices — otherwise drop the numbers
- Remove the expired July 25 bundle line (`deadline-note`)

### 10. Add an FAQ section
Cover: venue address & parking · lunch/refreshments · what to bring · do you need a farm area picked · suitable for new agents · teams/brokerage groups · materials included · cancellation & ticket transfer · how bonuses are redeemed · payment plan availability.

---

## Tier 3 — Conversion mechanics

### 11. Sticky mobile register bar
`Sept. 22 | $1,000 + HST | Register` fixed to the bottom on mobile. Also add a 4th register button right after "What You'll Build" (currently only 3 CTA clusters on a very long page).

### 12. Checkout handoff (Square — off-page work)
- Rename the Square product to `Fast Track Farming — September 22, 2026` (currently "Farming 101 (Fast Track Program)")
- Show `$1,000 + HST` before the click
- Keep event image/branding on the Square page
- Remove or default the quantity step
- Show the refund/transfer policy before payment

### 13. Enquiry form — mostly done, verify
The review flagged a `mailto:` link. The page already uses a Google Form for "Request More Info" — so this is largely resolved. Remaining: confirm the form asks name / email / optional phone / question, and add a *"someone from Monica's team will reply within one business day"* line beside the button.

### 14. Measurement
- Meta Pixel is installed (`560295672672335`) and fires `InitiateCheckout` on CTA clicks — confirm a **Purchase** event actually fires on the Square thank-you side
- Google Analytics is not installed — add it
- Track: page visits → register clicks → checkout starts → purchases, plus enquiry submits, by campaign
- Add UTMs to every ad and preserve them through the Square handoff

---

## Metrics to watch
- Visitor → register-click rate
- Register-click → checkout-start rate
- Checkout-start → purchase rate
- Enquiry-form completion rate
- Registrations and cost per registration by campaign
- Drop-off between the Square event page and the payment form
