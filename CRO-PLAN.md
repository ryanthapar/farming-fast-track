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
`[x]` Done — see "Completed" note at the end of this item.

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

**Completed.** Hero now runs eyebrow → outcome H1 → deliverables sub → date → venue+price
→ CTA → reassurance line. The four badge pills were removed; their content is carried by the
reassurance line and the venue/price line. H1 resized to `clamp(34px,5.5vw,60px)` — the old
`clamp(46px,9vw,92px)` was set for a two-word title. Verified at 1280px and 390px.

Deliberately **not** changed, as they belong to other recos: the price still reads `$1,000`
(reco 3) and the secondary "See What's Inside" button was kept.

Side effect to be aware of: the replaced lead paragraph was the hero's only 6% mention, so
that claim is now gone from the hero. Reco 4 still owns the four remaining locations.

---

## 2. Place Monica's credibility near the top — Tier 1
`[x]` Done.

**Issue:** visitors scroll a long way before learning why Monica can command $1,000.

**Change:** compact credibility strip directly below the hero — `10+ yrs #1 REALTOR® in Etobicoke` · `1,700+ homes sold` · `$1B+ career volume` · `Top 0.1% of TRREB`. Follow with **one** strong testimonial carrying name, brokerage, photo and a specific result (Renee Proulx's $1M is the strongest candidate).

**Touches:** new `.cred` and `.proof` sections directly after `</header>`

**Completed.** Four-stat strip on a tinted band directly below the hero, followed by Renee
Proulx's testimonial in a card. 4-up on desktop, 2×2 on mobile.

Decisions taken:
- **About section left untouched** — its six-stat block still stands, so four numbers now
  appear twice on the page. Deliberate; reco 6 resolves it.
- **Sourcing notes moved to the footer** rather than sitting near the hero. The `†` (Etobicoke
  ranking) and `‡` (career totals) markers anchor down to `#source-etobicoke` and
  `#source-career` in the footer fineprint, matching how the existing `*` commission note
  already works. The `.about-note` text is now duplicated between the About section and the
  footer — also for reco 6 to consolidate.

**Photo:** supplied by Ryan and committed as `renee-proulx.jpg` — cropped from a 748px square
headshot to head-and-shoulders and resized to 320px so it reads clearly in the 74px circle.

**Note:** the page uses `*` for two different disclaimers — the commission note in the footer
and the Etobicoke sourcing note inside the About section. That collision is pre-existing, not
introduced here, and is worth cleaning up in reco 6.

---

## 3. Eliminate the price surprise — Tier 1
`[x]` Done.

**Issue:** the page says `$1,000` five times; Square charges `$1,130`. The $130 of HST appears for the first time at the payment screen.

**Change:** every price reference becomes `$1,000 + HST`.

| Line | Location | Current |
|---|---|---|
| 357 | Hero venue/price line | `Venu Event Space, Vaughan · $1,000 per seat` |
| 457 | "Who This Is For" close | `ready to invest $1,000` |
| 494 | Register — price anchor | `Ticket: $1,000` |
| 495 | Register — total value | `you pay $1,000` |
| 517 | "After August 16" card | `Same $1,000 — $3,000 less value` |

Plus a price line beside each registration button (lines 359, 522, 624).

*Line numbers refreshed after reco 1. The hero badge pill that used to hold the price is gone;
the hero price now lives in the venue line.*

**Leave alone:** the `$3,000` / `$4,000` bonus values — stated values, not charges.

**Completed.** All five references now read `$1,000 + HST`. The Register price anchor
additionally shows `($1,130 total)` on its own line beneath the headline figure — the one
place the exact charge appears, so it lands while the buyer is evaluating cost rather than at
the payment screen.

New `.cta-price` line added under the Register and final CTA button clusters:
`$1,000 + HST · Tuesday, September 22, 2026` (left-aligned variant in the final section to
match its layout). The hero needed no separate line — its price already sits directly above
the button in the venue line.

Verified: seven `$1,000` occurrences in the file, all carrying `+ HST`.

**Still outstanding for reco 10:** Square itself continues to reveal the $1,130 only at the
final stage. The page is now honest about it; the checkout is not yet.

---

## 4. Reframe the 6% commission language — Tier 1
`[~]` **Deferred — decision pending with Ryan.** Reviewed together Aug 10; coming back to it.

**Issue:** the body promises signing every listing at 6% while the footer disclaimer says no rate is guaranteed. The two fight each other.

**Change:** replace the promise with the approach — *learn how Monica presents her value, handles commission objections and defends her fee.*
- Curriculum step 12 (line 386): `Commission: Get 6% Every Time` → **Presenting Your Value & Holding Your Fee**
- "Hold your commission" card (line 430): drop *"so you sign at 6% every time"*
- Hero lead (line 357): *"signing every listing at 6%"* → the reframe
- Final CTA (line 622): *"sign at 6% every time"* → the reframe
- Meta descriptions (lines 8, 12) also carry the 6% claim
- Keep the footnote/disclaimer as is

### Current locations (line numbers as of Aug 10)

| Line | Where | Current |
|---|---|---|
| 444 | Curriculum step 12 | `Commission: Get 6% Every Time` |
| 488 | "Hold your commission" card | *"so you sign at 6% every time"* |
| 681 | Final CTA paragraph | *"the system to sign at 6% every time"* |
| 8 | `<meta name="description">` | *"the system to sign every listing at 6%"* |
| 12 | `<meta property="og:description">` | *"system to sign at 6% every time"* |

Line 716 (the footer disclaimer) stays as-is — it is the thing the rest of the page needs to
stop contradicting.

### Recommendation on the table

This is the largest substantive change in the plan and the one place worth pushing back on the
review slightly. "Sign at 6% every time" is the most concrete, most differentiating promise on
the page and is likely doing real conversion work with agents tired of discounting. The full
reframe is more credible and legally cleaner, but it is measurably softer copy.

Two options:

1. **Full reframe** (the review's recommendation) — remove the 6% promise everywhere; 6%
   survives only in the disclaimer as context for Monica's own practice.
2. **Middle path** — keep 6% but frame it as *Monica's* result rather than the buyer's
   guarantee. e.g. *"the exact conversation Monica uses to sign at 6% — and how to hold your
   own fee."* Retains the number's pulling power while removing the implied promise. Not
   proposed by the review.

**Claude's recommendation:** middle path for the two body locations (lines 488 and 681), and
the review's full rename for curriculum step 12 → **"Presenting Your Value and Holding Your
Fee."** A curriculum item reads as a promise about what *you* will achieve, which is where the
guarantee problem is sharpest. The meta descriptions should follow whichever way the body
copy goes.

This is a marketing judgment call for Ryan, not a technical one.

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

## Additional items — not from the review

Things spotted while working the list. Deferred by choice, not oversight.

### A1. Logo has a baked-in black background — Tier 1
`[ ]` **Deferred — fix later, confirmed with Ryan**

The hero logo (inline base64 PNG, `class="logo"`) renders as the *Let's Farm with Monica
Thapar* cloud sitting on a solid black rectangle instead of on the page background. The PNG
has black baked in rather than an alpha channel. Pre-existing — it is on the live page today
and was not introduced by any reco.

**Fix:** replace with a transparent-background PNG or SVG of the same logo. If no clean
source file exists, the black can be keyed out, though edge quality around the drop shadow
will need a look.

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
- Check the "Additional items" section above — A1 (logo background) is deliberately deferred
  and should either be done or consciously carried forward, not forgotten

---

## Metrics to watch

- Visitor → register-click rate
- Register-click → checkout-start rate
- Checkout-start → purchase rate
- Enquiry-form completion rate
- Registrations and cost per registration by campaign
- Drop-off between the Square event page and the payment form
