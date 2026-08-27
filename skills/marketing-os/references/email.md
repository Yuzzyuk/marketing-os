# Email

Email is the only channel the sender owns. It is also the channel where generic output is most fatal, because the reader granted access once and revokes it permanently. Every email must earn the next one.

Read `brand-context.md` first. Run every email through `slop-patterns.md` before delivery — inboxes are where AI-written prose gets caught fastest.

## Before writing anything

Establish, inferring where possible:
1. **Sequence type** — welcome, nurture, launch, re-engagement, abandonment, onboarding, sales follow-up
2. **What the reader just did** — the trigger event defines email 1 completely
3. **The one conversion goal** — a sequence with two goals achieves neither
4. **Sending reality** — list size, current open/click baseline, ESP. Skip if unavailable, but say projections are impossible without a baseline.

## Sequence architectures

Send counts and gaps are defensible defaults, not laws. Adjust to purchase-cycle length: a $9 app moves in days, a $50k contract moves in months.

### Welcome (5 emails, days 0 / 1 / 3 / 5 / 8)
1. **Deliver + one action.** Whatever was promised, instantly, plus the single next step. Highest open rate the sender will ever get — do not waste it on "thanks for subscribing."
2. **The story or the mechanism.** Why this exists, what it believes, why it works. Differentiation, not features.
3. **The best thing you have.** Strongest content, tool, or case study. Pure give.
4. **Objection email.** The #1 reason people don't buy, addressed head-on.
5. **Direct offer.** Clear ask, clear deadline or reason-to-act-now (real ones only).

### Nurture (6 emails, ~weekly)
Alternating give/ask at roughly 3:1. Each give must be independently worth the open — a "tip" that restates the blog post is an ask wearing a costume. Rotate angle families across sends (see `copy-frameworks.md`): problem → mechanism → proof → contrarian → identity → offer.

### Launch (8 emails across ~10 days)
1. Seed the problem (no product)
2. The mechanism / what's coming
3. Open — the announcement, full offer
4. Social proof + FAQ
5. Objection teardown
6. Case study or demo
7. Last-48h — restate offer, add nothing new
8. Final hours — shortest email of the sequence, one link

**Deadline integrity is non-negotiable.** If the cart doesn't actually close, do not say it closes. Fake urgency converts once and burns the list permanently. Cost-of-delay is the honest substitute.

### Re-engagement (3 emails)
1. "Still want these?" — genuine, not guilt
2. Best-of / what they missed
3. The breakup: explicit unsubscribe-by-inaction. **Actually remove non-responders.** A smaller engaged list outperforms a large dead one on every metric that matters, including deliverability of everything else you send.

## Subject lines

Generate 10+ per email using distinct angles, score with the copy panel (`copy.md`), pick the top and one contrast for testing.

- ~40 characters survive mobile truncation; front-load the payload
- Specific beats clever, and curiosity decays across a sequence — each curiosity subject spends trust the next one needs
- The preview text is the second subject line. Write it deliberately; never let "View this email in your browser" occupy it.
- Never write a subject the body doesn't cash. Open-rate won cheaply is click-rate lost.
- "Re:" and "Fwd:" fakery, ALL CAPS, and 🚨 are deliverability and trust liabilities, not tactics

## Body rules

- One goal, one primary link (repeated is fine; competing is not)
- Write to one person in their language — pull phrasing from reviews and support tickets when available
- First sentence must survive the preview pane standing alone
- Short paragraphs; the reader is on a phone in a queue
- Plain-text-feel outperforms designed templates for most B2B and creator sends; heavy design is for retail
- Sign as a person where the brand allows it
- The P.S. line gets read disproportionately — put the offer restatement or the human aside there, not nothing

## Deliverability floor

Not the specialist's depth, but never advise anything that breaks these:

- SPF, DKIM, DMARC must be set up before volume sending; if the user doesn't know, tell them to check first
- Never purchase lists, never scrape lists, no exceptions — beyond ethics, it destroys sender reputation for the whole domain
- Sunset non-openers on a schedule; engagement rate drives inbox placement
- Warm up new domains/IPs gradually; volume spikes from cold domains go to spam
- One-click unsubscribe present and honored — a legal requirement in most jurisdictions, and hiding it raises complaint rates, which is worse than the unsubscribe

## Output format

```
# [Sequence type] — [product]
Goal: [the one conversion] · Sends: [n] · Cadence: [days]

## Email 1 — [job of this email]
Subject: [chosen]
Alt subjects: [2, scored]
Preview: [text]
---
[Full body, ready to paste]
---
Send: day X · Segment/skip logic: [if any]

[... every email in full — never outline emails, write them ...]

## Testing plan
[One variable, which email, what a result would mean]

## Flagged
[Claims needing verification, deadlines needing confirmation, anything assumed]
```

## Metrics honesty

Open rates are unreliable post-privacy-changes (bot opens, prefetching inflate them). Weight clicks and replies over opens when judging results. Do not project revenue from a sequence that hasn't sent; give the levers instead. Sample-size discipline per `analytics.md` applies to every subject-line test.
