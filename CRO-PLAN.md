# Fast Track Farming — CRO Action Plan

Source: *Conversion Rate Optimization Review*, Pathmark Partners, Aug 4 2026.
Numbered 1–13 to match the document's "Detailed CRO Recommendations" exactly, so
"point 5" means the same thing in the plan and in the review. Each item carries a
**Tier** annotation for effort/risk — that's information, not running order.

- **Tier 1** — copy-only, low risk, ships immediately
- **Tier 2** — structural, needs new content written
- **Tier 3** — off-page work (Square, analytics) or new components

**Context:** the Aug 16 bonus deadline is 6 days out. Tier 1 items are high-confidence;
ship them rather than holding for a formal A/B test.

**Status key:** `[ ]` not started · `[~]` in progress · `[x]` complete

---

## 1. Rebuild the hero around the outcome — Tier 1
`[ ]`

**Issue:** "Fast Track Farming" is the event name, not an outcome. A visitor arriving from an ad has to interpret the offer before knowing if it's relevant.

**Change:** make the H1 outcome-led; result, audience, date, location, price and next action all visible within seconds.
- Eyebrow: `IN-PERSON WORKSHOP FOR GTA REALTORS®`
- H1: **Build Your Complete Geographic Farming Plan in One Day**
- Sub: leave with a defined farm, a written 12-step action plan, door-knocking scripts, a marketing calendar and the systems to begin immediately
- Details: `Tuesday, September 22, 2026 · 10:00 AM – 6:00 PM` / `Venu Event Space, Vaughan · $1,000 + HST`
- CTA: `REGISTER FOR SEPTEMBER 22`
- Reassurance: in person with Monica · written materials included · early-registration bonuses until Aug 16
- Keep "Fast Track Farming" as branding above or below the H1, not as the H1

**Touches:** `index.html` lines 343–365 (hero header)

---

## 2. Place Monica's credibility near the top — Tier 1
`[ ]`

**Issue:** visitors scroll a long way before learning why Monica can command $1,000.

**Change:** compact credibility strip directly below the hero — `10+ yrs #1 REALTOR® in Etobicoke` · `1,700+ homes sold` · `$1B+ career volume` · `Top 0.1% of TRREB`. Follow with **one** strong testimonial carrying name, brokerage, photo and a specific result (Renee Proulx's $1M is the strongest candidate).

**Touches:** new section after line 365; stats currently live at lines 470–477

---

## 3. Eliminate the price surprise — Tier 1
`[ ]`

**Issue:** the page says `$1,000` five times; Square charges `$1,130`. The $130 of HST appears for the first time at the payment screen.

**Change:** every price reference becomes `$1,000 + HST`.

| Line | Location | Current |
|---|---|---|
| 350 | Hero badge pill | `💵 $1,000 per seat` |
| 458 | "Who This Is For" close | `ready to invest $1,000` |
| 495 | Register — price anchor | `Ticket: $1,000` |
| 496 | Register — total value | `you pay $1,000` |
| 518 | "After August 16" card | `Same $1,000 — $3,000 less value` |

Plus a price line beside each `Reserve My Seat` button (lines 361, 523, 625).

**Open decision:** whether to show the full `$1,000 + HST ($1,130)` in the Register price anchor only, keeping `$1,000 + HST` everywhere else. Recommended.

**Leave alone:** the `$3,000` / `$4,000` bonus values — stated values, not charges.

---

## 4. Reframe the 6% commission language — Tier 1
`[ ]`

**Issue:** the body promises signing every listing at 6% while the footer disclaimer says no rate is guaranteed. The two fight each other.

**Change:** replace the promise with the approach — *learn how Monica presents her value, handles commission objections and defends her fee.*
- Curriculum step 12 (line 386): `Commission: Get 6% Every Time` → **Presenting Your Value & Holding Your Fee**
- "Hold your commission" card (line 430): drop *"so you sign at 6% every time"*
- Hero lead (line 357): *"signing every listing at 6%"* → the reframe
- Final CTA (line 622): *"sign at 6% every time"* → the reframe
- Meta descriptions (lines 8, 12) also carry the 6% claim
- Keep the footnote/disclaimer as is

---

## 5. Show what happens during the day — Tier 2
`[ ]`

**Issue:** 12 topics are listed but nothing shows how 8 hours are structured.

**Change:** add a timed agenda — farm plan → area selection → brand & marketing calendar → door-knocking demonstrations → lead tracking → follow-up → open houses → fee conversation → 30-day implementation plan. Include breaks and lunch.

**Also covers:** the "complete event details" gap — the page currently gives only "Venu Event Space" with no street address. Add full address, city, parking.

---

## 6. Shorten and reorganize the page — Tier 2
`[ ]`

**Issue:** ~11,000px on desktop, repeating "own a neighbourhood," "hold your commission," Monica's experience and "complete system."

**Change:** cut repetition, shorten Monica's bio and tie it to her ability to *teach* farming. Target sequence:

1. Outcome hero
2. Credibility strip
3. One powerful testimonial or short video
4. What attendees will leave with
5. The one-day agenda
6. Who this is for
7. Monica's abbreviated biography
8. Registration package and bonuses
9. Three detailed testimonials or case studies
10. FAQ
11. Final registration

**Note:** this is a rebuild, not an edit. Best done after points 1–4 are live.

---

## 7. Strengthen the social proof — Tier 2
`[ ]`

**Issue:** many names and quotes, but the strongest proof appears late and some is too general.

**Change:**
- Move the YouTube testimonial (line 560) near the top
- Build 3 short case studies: what they implemented, how long farming, measurable impact, photo, brokerage, farm area, verifiable profile
- The 21-name "Happy Farming Students" grid (lines 586–608) is weaker than 3 detailed stories — shrink it

---

## 8. Make the bonuses feel credible — Tier 2
`[ ]`

**Issue:** the `$3,000` bonus valuation and `$4,000` total value invite questions about how those numbers were set.

**Change:**
- Lead with what the private door-knocking session and post-event Zoom actually do for the attendee
- Keep the `$1,500 / $1,500` figures **only** if those services genuinely sell separately at those prices
- Remove the expired July 25 bundle reference (line 521)

---

## 9. Replace the email link with a proper enquiry form — Tier 3
`[ ]`

**Status:** largely already done. The review flagged a `mailto:` link, but the page now uses a Google Form for "Request More Info" (lines 525, 627).

**Remaining:** confirm the form asks name / email / optional phone / question, and add a *"a member of Monica's team will respond within one business day"* line beside the button.

---

## 10. Improve the checkout handoff — Tier 3
`[ ]`

**Issue:** checkout opens in a new tab, renames the event to "Farming 101 (Fast Track Program)", adds a quantity step, and reveals $1,130 only at the final stage.

**Change (Square-side, off-page):**
- Rename the product `Fast Track Farming — September 22, 2026`
- Show `$1,000 + HST` before the click
- Retain the event image and branding
- Remove or default the quantity step
- Show the refund/transfer policy before payment

**Also covers:** consistent event naming — "Fast Track Farming" everywhere, page and checkout.

---

## 11. Add a frequently asked questions section — Tier 2
`[ ]`

**Change:** concise FAQ covering —
- Exact venue address, and is parking included?
- Are lunch and refreshments provided?
- What should attendees bring?
- Do attendees need a farming area selected already?
- Is it appropriate for newer agents?
- Can teams or brokerage groups attend?
- What materials are included?
- What is the cancellation / ticket-transfer policy?
- How and when are bonuses redeemed?
- Is a payment-plan option available?

---

## 12. Add a persistent mobile registration button — Tier 3
`[ ]`

**Issue:** only three CTA clusters across a very long page (lines 361, 523, 625), leaving long stretches where a visitor can't act.

**Change:** sticky mobile bar reading `Sept. 22 | $1,000 + HST | Register`. Add a fourth registration button after "What You'll Build" (after line 395).

---

## 13. Strengthen measurement and follow-up — Tier 3
`[ ]`

**Issue:** Meta Pixel is installed (`560295672672335`, line 27) and fires `InitiateCheckout` on CTA clicks, but no confirmed registration conversion event. No Google Analytics.

**Change:**
- Confirm a **Purchase** event fires on the Square completion side
- Install Google Analytics
- Track: visits → register clicks → checkout starts → purchases, plus enquiry submissions, by campaign
- Add UTM parameters to every ad and preserve attribution through the Square handoff

---

## 14. Final review — after all items are complete
`[ ]`

Once points 1–13 are marked complete, do a full review pass before calling the work done:

- Re-read the original Pathmark document end to end against the live page; confirm every recommendation was either implemented or consciously declined, with the reason recorded here
- Check nothing was missed from the document's "Highest-Priority Opportunities" summary — it contains two items with no numbered recommendation of their own: **complete event details** (folded into 5 and 11) and **consistent event naming** (folded into 10)
- Verify no `$1,000` without `+ HST` survives anywhere, including meta tags and the Square page
- Verify no unqualified 6% promise survives anywhere, including meta descriptions and OG tags
- Walk the full funnel as a buyer would: ad → landing page → register click → Square → payment → confirmation, on both desktop and mobile
- Confirm every internal anchor, CTA link and tracking event still fires after the reorganization in point 6
- Note anything deferred or descoped so it doesn't quietly disappear

---

## Metrics to watch

- Visitor → register-click rate
- Register-click → checkout-start rate
- Checkout-start → purchase rate
- Enquiry-form completion rate
- Registrations and cost per registration by campaign
- Drop-off between the Square event page and the payment form
