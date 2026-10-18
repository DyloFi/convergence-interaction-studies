# loar-level01: The Law of Accelerating Returns, Level 01

Source: HTML and Markdown export of a Claude artifact, "CONVERGENCE · Level 01 — The Law of Accelerating Returns", saved 18 Oct 2026.
Files: loar-level01.html (1,202,933 bytes) and loar-level01.md (7,284 bytes, page text only).
SHA-256 of the HTML: 7308d5e70c99b0157521013282c59cf5b081bfeeba4ba0a76b61e6de32983ad0
Both files are byte-identical to the export. Do not edit them; copy to work on them.

## Why it is here
It is the example of the kind of interactive storytelling the Convergence site should use eventually: one pinned stage, where scroll drives a drawing that builds up layer by layer. It is a reference only. It is not meant for the Fourth Turning page or any specific page.

## How it works (read from the code)
- No libraries. Plain JavaScript, SVG and CSS. The only outside load is Google Fonts.
- A tall track (560vh) holds one sticky, screen-sized stage. Nothing scrolls away.
- Scroll becomes one number p from 0 to 1. One function runs each animation frame and sets every layer from p. Beats start at p = 0, .06, .20, .40, .56, .74, .92 and 1.
- Lines draw on by animating stroke-dashoffset on SVG paths (ramp, straight line, S-curves, envelope).
- The pencil drawing reveals through a clip-path that sweeps up, with a cut line riding the edge. The title writes on left to right the same way.
- 64 small walkers sit along the ramp path. The number shown is 2 to the power of (6 x p), so the crowd doubles as you scroll.
- Five discs spread and light up one by one. Anchors A to D fade in at set points.
- One margin note shows at a time and writes on over about half a second. The ruler ticks are buttons that jump to a beat.
- A 1.3 second intro plays on load. Reduced motion skips it.
- A second script drives the "Read the ramp" section after the plate: a small copy of the ramp, four chapters A to D, a figure that walks the ramp as you scroll, and a readout that updates per chapter.
- A research drawer (REF 01 to 05) shows claim, argument and the repo file path for each reference. A sheet viewer opens 19 embedded report sheets with prev and next.
- Hidden keys: D opens the drawer, G toggles the grid, Esc closes. A crosshair follows the mouse and reads out drawing coordinates (mouse only).

## What to reuse
The mechanics: sticky track, single progress value with per-layer start and end points, stroke-dashoffset draws, clip sweeps, elements that multiply with progress, a ruler or gauge tied to progress, source drawers tied to repo files, a tag for unverified claims.

## What is content-specific
All text, the ramp drawing, the paradigm staircase drawing, the 19 sheets (most of the file size) and the anchor positions on the ramp path.

## Look
Warm paper (#F6F3EC) and near-black ink, with one chartreuse accent (#C9DB5A) used as marker washes and a muted red-brown (#9A3E2F) used only for the [UNVERIFIED] tag. Dark mode flips to a dark ground. Fonts: Big Shoulders Stencil, Architects Daughter, Newsreader, IBM Plex Mono. The convergenceweb site is monochrome, so colour use is an open decision.

## Not verified
Seen as still screenshots only (headless Chrome at set scroll points), plus the code. The easing, timing and hover crosshair have not been watched in motion. The stylesheet was only partly read, so frame grid, dark mode and reduced-motion rules come from partial reading.
