# Punt · PLY-001 — Getting them in the door (POC)

An interactive proof-of-concept for **explaining the unified wallet and Gold Coins vs. Sweeps
Coins at the moment of confusion**, in an audience-appropriate voice, so a first-time Play
registrant reaches a first play instead of bouncing. A single self-contained HTML file — no
build step, no dependencies.

## View it

Open [`index.html`](index.html) (or
[`ply-001-currency-comprehension.html`](ply-001-currency-comprehension.html)) in any modern
browser.

## The shape

- **Landing** — the Punt **Play lobby** board (masthead with the Punt wordmark, featured hero,
  welcome-bundle side panel, game grid) is the starting point. It's what's on screen first — no
  modal — for a **2-second beat** before the currency explanation auto-prompts, so it reads as
  arriving into the lobby rather than being gated by a dialog. Tap the board early to skip the
  wait. On **desktop** it fades/rises in, matching the rest of the flow; on **mobile** it slides
  up from the bottom like a native drawer, clipped to the simulated device frame so it never
  visibly spills past the phone's edges. The modal never scrolls internally on either device —
  no scrollbar ever appears.
- **The moment** — the currency explanation opens in a **modal overlaying the board**, the way
  a first-timer would meet it in the real product. Reopen it anytime from the wallet-setup CTA,
  the side-panel "See the difference" link, or the masthead.
- **Trade CTAs carry the currency choice through** — every "Trade" button on the board (the
  hero market and each featured card) is now two buttons, **"Trade with Gold Coins"** and
  **"Trade with Sweeps Coins"**, so the two-currency distinction the modal just taught doesn't
  disappear the moment you leave it. The hero's pair sits side by side on desktop (collapsing to
  stacked on mobile, matching the board's own responsive breakpoint); the featured cards stay
  stacked at every size.
- **Reset flow** closes the modal and re-triggers the same board-first, 2-second auto-prompt
  used on load, rather than snapping straight back to it.

## The brief

- **Proves Bet 1** — premium is the price of entry; reads through to Bet 3, a single *player
  profile* served by platform-owned onboarding, not a bolted-on disclosure.
- **Moves CAC ↓** — bounce rate at the currency-explanation moment and share of new
  registrations reaching first play are the primary signals.
- **Comprehension, not pricing or trust** — a first-timer hits two currencies in one unified
  wallet and can't tell them apart. Isolated to comprehension only.
- **Scope** — Play room and unified-wallet ADW onboarding.

## The scenario

One first-time Play registrant. On sign-up a **welcome bundle** drops both currencies into a
single wallet — **10,000 Gold Coins** (for fun) and **5 Sweeps Coins** (for prizes) — and the
two look confusingly alike. Success = the difference lands well enough that the player reaches
a **first play**, and could explain it in their own words.

## The concept

**The Analogy** — audience-appropriate metaphor. Explains the two coins through something the
player already knows — an arcade. Gold Coins are the tokens you play with; Sweeps Coins are the
tickets you trade for a prize. Warm, plain, zero legalese.

## Using the prototype

A bottom **REVIEW bar** (shared Punt POC format) drives everything:

- **Fidelity** — Mid-Fi (light editorial mono) / Hi-Fi (dark brand skin).
- **Device** — Desktop / Mobile (wraps the board in a phone frame).
- **Reset flow** — restart the flow · **UX notes** — right-hand drawer with the pattern
  rationale and considerations.

## Deliberately not built

Per the hard constraints: no pricing or trust framing, and no default to generic
legal/compliance-style currency copy. The explanation stays isolated to comprehension.

## Status

Internal POC — happy-path flows only. Board content, balances, the game list, and the
welcome-bundle values are illustrative placeholders where real wallet and game data would sit.

## Deploy

This repo is connected to the **punt-ply-001** Vercel project — every push to `main` deploys
automatically. No build step; Vercel serves the static HTML as-is.
