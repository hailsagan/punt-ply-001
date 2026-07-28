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

- **Landing** — the Punt **Play lobby** board (utility nav, newspaper masthead, featured hero,
  welcome-bundle side panel, game grid) is the starting point.
- **The moment** — the currency explanation opens in a **modal overlaying the board**, the way
  a first-timer would meet it in the real product. Reopen it anytime from the wallet-setup CTA,
  the side-panel "See the difference" link, or the masthead.
- **Concepts** — the modal content switches between the two concepts below.

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

## The concepts

| # | Concept | Pattern |
|---|---------|---------|
| V1 | The Split | Glanceable side-by-side — both coins contrasted in the wallet, one plain line each |
| V3 | The Analogy | Audience-appropriate metaphor — arcade tokens (Gold) vs. prize tickets (Sweeps) |

## Using the prototype

A bottom **REVIEW bar** (shared Punt POC format) drives everything:

- **Concept** — switch between V1 and V3; the modal reopens on the chosen concept.
- **Fidelity** — Mid-Fi (light editorial mono) / Hi-Fi (dark brand skin).
- **Device** — Desktop / Mobile (wraps the board in a phone frame).
- **Reset flow** — restart the current concept · **UX notes** — right-hand drawer with the
  pattern rationale and considerations per concept.

## Deliberately not built

Per the hard constraints: no pricing or trust framing, and no default to generic
legal/compliance-style currency copy. The explanation stays isolated to comprehension.

## Status

Internal POC — happy-path flows only. Board content, balances, the game list, and the
welcome-bundle values are illustrative placeholders where real wallet and game data would sit.
