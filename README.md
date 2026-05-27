# Gig Worker Social Protection — Prototype

A clickable, mobile-first prototype of a service for the **National Insurance Scheme of Barbados**, designed to help gig workers, freelancers, platform workers, and self-employed Barbadians understand and access NIS protection.

**Live prototype:** _link added once GitHub Pages finishes building_

---

## What this is

An early-stage Alpha prototype intended for **user testing and stakeholder demos**. Not a production service. Not connected to real NIS systems. No personal data is stored — the "submit" step is simulated.

The tone is deliberately **protective, voluntary, and supportive** — never enforcement, surveillance, or compliance-focused.

## The flow

1. **Landing** — what the service is, who it's for, what NIS protects you against
2. **How you earn** — choose the description that fits (delivery, freelance, remote, rental, casual, other)
3. **How NIS protects you** — five benefit cards explained in plain language
4. **Contribution estimator** — a slider + income variability question → estimated monthly range
5. **Tell us where to reach you** — short interest form with trust messaging
6. **Confirmation** — reference number + what happens next

## Running locally

It's a single self-contained HTML file. Just open it:

```bash
open index.html
```

Or serve it (for accurate mobile testing on a phone on the same network):

```bash
python3 -m http.server 8000
# then visit http://localhost:8000 or http://<your-mac-ip>:8000 from a phone
```

## Tech

- Single static HTML file — no build step, no dependencies
- Tailwind CSS via CDN
- Figtree font via Google Fonts
- Uses the [alpha.gov.bb](https://alpha.gov.bb) design tokens (`bb-`-prefixed colours, spacing, typography)

## User testing prompts

Suggested starter questions:

- "Without reading every word on this first screen, tell me what this service does."
- "Which of these descriptions sounds most like the work you do?" _(worker-type screen)_
- "If you had to put in around $75 a month, how would that feel?"
- "What, if anything, would stop you from submitting this form?"
- "Where would you expect to go next?" _(confirmation screen)_

Watch for: hesitation on the estimator (financial anxiety), distrust of the contact field, confusion at "Already registered with NIS?".

## Feedback

Open an issue with what you saw, who you tested with, and what they said.

---

A GovTech Barbados project. Built on the [alpha.gov.bb](https://alpha.gov.bb) design system.
