# Fast Track Farming — CRO Action Plan

Source: *Conversion Rate Optimization Review*, Pathmark Partners, Aug 4 2026.

Numbered **1–13 to match the review's "Detailed CRO Recommendations" exactly**, so "reco 5"
means the same thing in this plan and in the source document. Items 14 and A1 are ours.

Each item carries a **Tier** annotation for effort/risk. That's information, not running order:

- **Tier 1** — copy-only, low risk, ships immediately
- **Tier 2** — structural, needs new content written
- **Tier 3** — off-page work (Square, analytics) or new components

**Status key:** `[ ]` not started · `[~]` in progress / decision pending · `[x]` complete

> **A note on references.** This file deliberately avoids `index.html` line numbers — recos 5
> and 6 moved several hundred lines and made every previous citation wrong. Sections are
> identified by heading text, `id`, or CSS selector instead, which survive reordering.

---

## Status at a glance

| # | Recommendation | Tier | Status |
|---|---|---|---|
| 1 | Rebuild the hero around the outcome | 1 | `[x]` |
| 2 | Place Monica's credibility near the top | 1 | `[x]` |
| 3 | Eliminate the price surprise | 1 | `[x]` |
| 4 | Reframe the 6% commission language | 1 | `[x]` |
| 5 | Show what happens during the day | 2 | `[x]` |
| 6 | Shorten and reorganize the page | 2 | `[x]` |
| 7 | Strengthen the social proof | 2 | `[ ]` |
| 8 | Make the bonuses feel credible | 2 | `[x]` |
| 9 | Replace the email link with an enquiry form | 3 | `[ ]` mostly pre-done |
| 10 | Improve the checkout handoff | 3 | `[ ]` Square-side |
| 11 | Add an FAQ section | 2 | `[x]` |
| 12 | Add a persistent mobile registration button | 3 | `[x]` |
| 13 | Strengthen measurement and follow-up | 3 | `[ ]` |
| A1 | Logo has a baked-in black background | 1 | `[ ]` deferred |
| 14 | Final review pass | — | `[ ]` |

### What shipped on `claude/landing-page-edits-w5j1g9`

Recos 1–6, 8, 11 and 12. Net effect on the page:

- Hero leads with the outcome, not the event name; event name moved to the eyebrow
- Credibility strip and Renee Proulx's testimonial now sit directly below the hero
- Every price reads `$1,000 + HST`, with `($1,130 total)` shown once in the Register section
- 6% reframed throughout as Monica's own result rather than the buyer's guarantee
- New one-day agenda section; venue address and parking added to the details bar
- Photo gallery moved out of last position; page 11.5% shorter by density
- Bonuses lead with what the attendee gets, with the expired July 25 reference removed
- New FAQ section answering all ten of the review's questions
- Sticky mobile registration bar, plus a fourth CTA after "What You'll Build"

### Current section order

1. Hero
2. Credibility strip (`.cred`)
3. Renee's testimonial (`.proof`)
4. What You'll Build (`#curriculum`)
5. The One-Day Agenda (`#agenda`)
6. See It In Action (`.gallery`)
7. Look At Who's Winning (`.why`)
8. Who This Is For (`#who-for`)
9. About Monica Thapar (`.about`)
10. Register & Get More (`#register`)
11. Details bar (`.details--slate`)
12. From Agents Who Farm (testimonials + video)
13. Happy Farming Students
14. Frequently Asked Questions (`#faq`)
15. Ready to Farm Your Area? (`.final`)

---

## 1. Rebuild the hero around the outcome — Tier 1
`[x]` **Complete**

**Issue:** "Fast Track Farming" is the event name, not an outcome. A visitor arriving from an
ad had to interpret the offer before knowing whether it was relevant.

**Shipped.** The hero now runs eyebrow → outcome H1 → deliverables sub → date → venue + price
→ CTA → reassurance line.

- Eyebrow: `Fast Track Farming · In-Person Workshop for GTA REALTORS®`
- H1: **Build Your Complete Geographic Farming Plan in One Day**
- Sub lists what you physically leave with: defined farm, written 12-step plan, door-knocking
  scripts, marketing calendar, systems
- CTA reworded to `Register for September 22`
- Reassurance line: in person with Monica · written materials included · early-registration
  bonuses until August 16

The four badge pills were removed; their content is carried by the reassurance and venue
lines. H1 resized from `clamp(46px,9vw,92px)` to `clamp(34px,5.5vw,60px)` — the old size was
set for a two-word title. Verified at 1280px and 390px.

**Decisions:** the secondary "See What's Inside" button was kept even though the review's copy
shows a single CTA — it is a scroll link and doesn't compete for the click.

**Side effect:** the replaced lead paragraph was the hero's only 6% mention, so that claim left
the hero as a consequence of the restructure. Reco 4 handled the rest.

---

## 2. Place Monica's credibility near the top — Tier 1
`[x]` **Complete**

**Issue:** visitors scrolled roughly 40% of the page before learning why Monica can command
$1,000.

**Shipped.** A four-stat strip on a tinted band directly below the hero — `10+ yrs` #1 in
Etobicoke, `1,700+` career homes sold, `$1B+` career volume, `Top 0.1%` of TRREB. 4-up on
desktop, 2×2 on mobile. Below it, Renee Proulx's testimonial in a card with her photo,
brokerage and a specific result ("$1 million in the last two years").

**Photo:** supplied by Ryan, committed as `renee-proulx.jpg` — cropped from a 748px square
headshot to head-and-shoulders and resized to 320px so it reads clearly in the 74px circle.

**Decisions:** the About section was left untouched at Ryan's direction, so four of these
numbers appear twice on the page. Still true after reco 6 — Ryan declined the cuts.

---

## 3. Eliminate the price surprise — Tier 1
`[x]` **Complete**

**Issue:** the page said `$1,000` five times; Square charges `$1,130`. The $130 of HST first
appeared at the payment screen.

**Shipped.** All five references now read `$1,000 + HST`:

| Location | Now reads |
|---|---|
| Hero venue/price line | `Venu Event Space, Vaughan · $1,000 + HST per seat` |
| "Who This Is For" close | `ready to invest $1,000 + HST` |
| Register price anchor | `Ticket: $1,000 + HST` |
| Register total value | `you pay $1,000 + HST` **($1,130 total)** |
| "After August 16" card | `Same $1,000 + HST — $3,000 less value` |

`($1,130 total)` appears exactly once, in the Register price anchor, so the real charge lands
while the buyer is evaluating cost rather than at the payment screen.

A new `.cta-price` line sits under the Register and final CTA button clusters:
`$1,000 + HST · Tuesday, September 22, 2026`. The hero needed none — its price already sits
directly above the button.

**Left alone:** the `$3,000` / `$4,000` bonus values — stated values, not charges.

**Verified:** every `$1,000` occurrence in the file carries `+ HST`.

**Still open, for reco 10:** Square continues to reveal $1,130 only at the final stage. The
page is now honest about the total; the checkout is not yet.

---

## 4. Reframe the 6% commission language — Tier 1
`[x]` **Complete** — Ryan chose the middle path

**Issue:** the body promised signing every listing at 6% while the footer disclaimer said no
rate is guaranteed. The two contradicted each other, and the contradiction was most visible to
the careful readers least likely to spend $1,000 on a page they distrust.

**The decision.** Two options were put to Ryan: the review's full reframe (remove 6%
everywhere), or a middle path keeping 6% as *Monica's* result rather than the buyer's
guarantee. Ryan chose the middle path.

**Shipped:**

| Where | Now reads |
|---|---|
| Curriculum step 12 | **Presenting Your Value & Holding Your Fee** (full rename) |
| "Hold your commission" card | *"Step 12 is that exact conversation — the one Monica uses to sign at 6%\*, and how to hold your own fee."* |
| Final CTA | *"…the fee conversation Monica uses to sign at 6%\* — and how to hold your own."* |
| `<meta name="description">` | *"…the fee conversation Monica uses to sign at 6%."* |
| `<meta property="og:description">` | *"…the fee conversation Monica uses to sign at 6%."* |

Step 12 got the review's **full rename** rather than the middle path: every other curriculum
item names a skill or deliverable, so a promise about the buyer's future rate was both the
sharpest form of the guarantee problem and the most out of place in that list.

A `*` disclaimer link was added to the "hold your commission" card, which previously asserted
6% with no pointer to the footnote. Both body mentions now link to `#commission-note`.

The footer disclaimer is unchanged and now agrees with the body copy — it already said Fast
Track Farming "teaches an approach to presenting and holding your fee."

**Result:** four 6% mentions remain (two body, two meta), all framed as Monica's practice, plus
the disclaimer. No unqualified promise survives.

---

## 5. Show what happens during the day — Tier 2
`[x]` **Complete**

**Issue:** 12 topics were listed but nothing showed how eight hours are structured.

**Shipped.** New `#agenda` section after the curriculum, built from Ryan's *Farming 101 –
FASTTRACK Proposed Agenda*. 17 rows on a two-column timeline running 10:00 AM to 5:45 PM, with
both breaks and lunch styled as muted rest rows. Times derived from the source document's
minute counts, rounded, with a note that they are approximate.

The details bar went from three columns to four: Place carries the full address
(**2800 Hwy 7, Vaughan, ON L4K 1W8**) and a new Parking column reads "Free & ample on site".

**Lunch is provided** — confirmed by Ryan. Stated on the agenda row and in the note beneath.

**Deliberately omitted from the public agenda** — internal planning items that would read badly
to a prospective buyer:

- **"Course Offer" ×4** — publishing that the day contains four sales pitches would work
  directly against registration
- **Sponsor slots** attached to the three role-play blocks
- **"Stand-Up Exercise"** labels — internal shorthand for delivery format

Nothing was invented: every published row maps to a real item in the source. The review's
suggested "30-day implementation plan" was **not** added, because the source agenda does not
contain one — it closes with mindset and next steps.

**Also closes** the "complete event details" gap from the review's priority summary.

---

## 6. Shorten and reorganize the page — Tier 2
`[x]` **Complete** — reorder + density; content cuts declined

**Issue:** the review measured ~11,000px on desktop with four ideas repeating.

**Finding worth keeping.** The page was already in the review's recommended sequence — hero →
credibility → proof → what you get → agenda → who it's for → bio → registration → testimonials
→ close all matched. The only section out of place was the photo gallery, sitting *after* the
final CTA.

**Shipped:**

- **Reorder:** "See It In Action" moved from last to directly after the agenda. "Ready to Farm
  Your Area?" now genuinely closes the page.
- **Density**, since Ryan declined the content cuts:

| Change | |
|---|---|
| `section` padding | 66px → 46px (mobile 48px → 34px) |
| `.hero` padding | 56/60px → 40/44px |
| Curriculum + student grids | 2 columns → 3 desktop, 2 tablet, 1 mobile |
| Block top margins | 42px → 30px, 34px → 26px throughout |
| Callouts, card padding, agenda rows | tightened 15–25% |

**Result: 13,109px → 11,605px at 1280px wide — 1,504px shorter, an 11.5% reduction**, with
nothing removed. Mobile still stacks single-column.

- **All disclaimers consolidated into the footer**, per Ryan, under four distinct symbols with
  every in-body marker anchoring to them:

| Symbol | Note | Anchor |
|---|---|---|
| `*` | Commission / 6% disclaimer | `#commission-note` |
| `†` | #1 in Etobicoke — R E Stats / TRREB sourcing | `#source-etobicoke` |
| `‡` | Career totals as of June 2026 | `#source-career` |
| `§` | Student results vary | `#source-students` |

  `.about-note` and `.students-note` were removed from the body along with their now-unused
  CSS. This resolved a pre-existing collision where `*` meant two different things depending on
  where you were on the page.

**Explicitly declined by Ryan, still available later:** shortening Monica's bio, removing the
duplicate stats, cutting "Look At Who's Winning" and the 21-name student grid. The review's
core complaint was volume, and density addressed roughly a third of it.

---

## 7. Strengthen the social proof — Tier 2
`[ ]` **Not started** — needs content from Ryan

**Issue:** many names and quotes, but the strongest proof appears late and some is too general.

**Change:**
- Move the YouTube testimonial (the `.video` figure in "From Agents Who Farm") near the top
- Build 3 short case studies: what they implemented, how long they have been farming,
  measurable impact, photo, brokerage, farm area, verifiable profile
- The 21-name "Happy Farming Students" grid is weaker than three detailed stories — shrink it

**Blocker:** the case studies don't exist yet. Needs names, results and photos from Ryan.
Note that reco 2 already moved one strong testimonial (Renee) to the top, which partially
satisfies the "strongest proof appears late" half of this item.

---

## 8. Make the bonuses feel credible — Tier 2
`[x]` **Complete**

**Issue:** the `$3,000` bonus valuation and `$4,000` total value invite questions about how
those numbers were set.

**Change:**
- Lead with what the private door-knocking session and post-event Zoom actually do for the
  attendee
- Keep the `$1,500 / $1,500` figures **only** if those services genuinely sell separately at
  those prices — needs Ryan's confirmation
- Remove the expired July 25 bundle reference (`.deadline-note` in the Register section)

**Shipped.** Both bonuses now lead with the practical benefit; the dollar value follows on a
muted meta line rather than sitting beside the title. Ryan confirmed both services genuinely
sell at $1,500, so the figures were retained.

Facts confirmed by Ryan and now stated on the page, which is what makes the values credible:

| | Door-knocking session | Zoom implementation session |
|---|---|---|
| Format | One-on-one with Monica | Group, on Zoom |
| Where | Monica's own Etobicoke farm | — |
| Attendee role | Knocks doors themselves, gets live feedback | Brings their own farm's challenges |
| Timing | Redeemable within one year | Four weeks after the event, 90 minutes |
| Who's on it | Monica | Monica, plus Ricardo (her right hand in real estate for 15 years) and Ryan (operations, team and growth) |

**Copy.** Ryan chose option 1A for the door-knocking session and 2B for the Zoom session, from
three drafted per bonus. 1A's closing line — *"One hour in the field teaches what a day in a
classroom can't"* — was replaced at Ryan's direction because it diminished the workshop being
sold. It now reads *"It is where everything you build at the workshop meets a real doorstep,"*
positioning the bonus as application of the day rather than a substitute for it.

**Naming:** first names only for Ricardo and Ryan, per Ryan. Deliberate — do not "correct" to
full names later.

**The July 25 line** now reads "Bonus deadlines are firm — this bundle closes August 16",
keeping the firmness without referencing an expired offer.

---

## 9. Replace the email link with a proper enquiry form — Tier 3
`[ ]` **Mostly pre-done**

**Status:** the review flagged a `mailto:` link, but the page already uses a Google Form for
"Request More Info" (the `.btn-soft` buttons in the Register and final CTA clusters).

**Remaining:** confirm the form asks name / email / optional phone / question, and add a
*"a member of Monica's team will respond within one business day"* line beside the button.

---

## 10. Improve the checkout handoff — Tier 3
`[ ]` **Not started** — Square-side, off-page

**Issue:** checkout opens in a new tab, renames the event to "Farming 101 (Fast Track
Program)", adds a quantity step, and reveals $1,130 only at the final stage.

**Change:**
- Rename the product `Fast Track Farming — September 22, 2026`
- Show `$1,000 + HST` before the click
- Retain the event image and branding
- Remove or default the quantity step
- Show the refund / transfer policy before payment

**Also covers** consistent event naming — "Fast Track Farming" everywhere, page and checkout.

---

## 11. Add a frequently asked questions section — Tier 2
`[x]` **Complete**

**Shipped.** New `#faq` section between "Happy Farming Students" and the final CTA, built as
native `<details>`/`<summary>` accordions — no JavaScript, keyboard accessible, and collapsed
by default so ten questions cost ~500px rather than ~1,600px.

All ten answers confirmed by Ryan:

| Question | Answer |
|---|---|
| Venue and parking | 2800 Hwy 7, Vaughan; free and ample on site |
| Lunch and refreshments | Lunch provided; two breaks built in |
| What to bring | Laptop only — workbook and pen provided |
| Farming area needed beforehand? | No, choosing one is step 2; helps to arrive with 2–3 in mind |
| Suitable for newer agents? | Yes — all experience levels, brand new to seasoned |
| Teams / brokerage groups | Yes; reach out about brokerage programs |
| Materials included | 12-step plan, scripts, flyers/giveaways calendar, workbook and pen, 1-month "No Chai Samosa" membership |
| Cancellation / transfer | **Non-refundable and non-transferable** |
| Bonus redemption | Team reaches out post-event to book the door-knocking session; Zoom link sent 5 days before the session |
| Payment plans | None — paid in full at checkout |

**Judgment call on the cancellation answer.** A flat "no refunds, no transfers" is friction, and
this reco exists to reduce friction. It is stated plainly rather than softened — burying it
would just move the problem to the customer-service inbox — but the answer pairs it with the
existing 15-minute call with Monica: *"If you're not certain the workshop is right for you,
book a call before you register."* That turns a dead end into a next step without misrepresenting
the policy.

**Cost to page height:** 13,109px was the pre-reco-6 baseline; the page is now 12,820px —
still below where it started, with a whole FAQ added.

---

## 12. Add a persistent mobile registration button — Tier 3
`[x]` **Complete**

**Issue:** three CTA clusters across a long page — hero, Register, final — leaving long
stretches where a visitor can't act.

**Shipped.**

- **`.sticky-cta`** — fixed bottom bar, mobile only (`max-width:720px`), reading `Sept. 22 /
  $1,000 + HST` with a `Register` button. Slate background, fires the same
  `InitiateCheckout` pixel event as every other registration button. Respects
  `env(safe-area-inset-bottom)` for iPhone home-indicator clearance, and `body` carries a
  76px bottom padding on mobile so the bar never covers the footer disclaimers.
- **Fourth CTA** after "What You'll Build", before the membership callout, with the standard
  `.cta-price` line beneath it.

**Decision:** the bar is always visible on mobile rather than appearing after a scroll
threshold. That would need JavaScript, and the page currently ships none of its own. Visible-
always is marginally redundant at the very top of the page and completely robust everywhere
else.

**Registration touchpoints are now five on mobile** (sticky bar, hero, post-curriculum,
Register section, final CTA) and four on desktop.

---

## 13. Strengthen measurement and follow-up — Tier 3
`[ ]` **Not started**

**Issue:** the Meta Pixel (`560295672672335`) is installed in `<head>` and fires
`InitiateCheckout` on CTA clicks, but no registration conversion event is confirmed. No Google
Analytics.

**Change:**
- Confirm a **Purchase** event fires on the Square completion side
- Install Google Analytics
- Track: visits → register clicks → checkout starts → purchases, plus enquiry submissions, by
  campaign
- Add UTM parameters to every ad and preserve attribution through the Square handoff

**Sequencing note:** recos 1–6 changed the hero, the price presentation and the page's whole
persuasion order. Without this item, there is no way to measure whether any of it helped.
Worth doing before or immediately after the first merge to production, not last.

---

## Additional items — not from the review

Spotted while working the list. Deferred by choice, not oversight.

### A1. Logo has a baked-in black background — Tier 1
`[ ]` **Deferred — confirmed with Ryan, fix later**

The hero logo (inline base64 PNG, `class="logo"`) renders as the *Let's Farm with Monica
Thapar* cloud on a solid black rectangle instead of on the page background. The PNG has black
baked in rather than an alpha channel. Pre-existing — live on the current page, not introduced
by any reco.

**Fix:** replace with a transparent-background PNG or SVG. If no clean source exists, the black
can be keyed out, though edge quality around the drop shadow will need a look.

---

## 14. Final review — after all items are complete
`[ ]`

Once 1–13 are resolved, do a full pass before calling the work done:

- Re-read the Pathmark document end to end against the live page; confirm every recommendation
  was implemented or consciously declined, with the reason recorded here
- Check the review's "Highest-Priority Opportunities" summary — it contains two items with no
  numbered recommendation of their own: **complete event details** (closed in reco 5) and
  **consistent event naming** (belongs to reco 10)
- Verify no `$1,000` without `+ HST` survives anywhere, including meta tags and Square
- Verify no unqualified 6% promise survives anywhere, including meta and OG tags
- Walk the full funnel as a buyer: ad → landing page → register click → Square → payment →
  confirmation, on desktop and mobile
- Confirm every internal anchor, CTA link and tracking event still fires
- Confirm the four footer disclaimer symbols still match their in-body markers
- Check A1 above — deliberately deferred, should be done or consciously carried forward
- Note anything deferred or descoped so it doesn't quietly disappear

---

## Metrics to watch

- Visitor → register-click rate
- Register-click → checkout-start rate
- Checkout-start → purchase rate
- Enquiry-form completion rate
- Registrations and cost per registration by campaign
- Drop-off between the Square event page and the payment form
