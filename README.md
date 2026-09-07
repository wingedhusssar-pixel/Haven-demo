# Haven

A peer-connection app built to fight loneliness and mental health. Haven matches verified users on
shared interests and background, gives them group spaces and safe ways to meet in
person, and puts a serious safety system at the center of the product rather than
bolting it on.

This repo is the interactive front-end prototype: a single self-contained
`index.html` that runs the whole product as a clickable demo, no backend
required.

**Live demo:** https://haven-demo.vercel.app

> **Scope, stated plainly.** Haven was built as a prototype for the Bada Macha
> Venture Pitch Competition (3rd place, international finalist). It is a
> front-end product prototype, not a production app. The data is seeded, state
> lives in the browser for the session, and the safety flows (identity
> verification, the pattern detectors) are demonstrated with scripted
> simulations to show how the system behaves, not a live backend. The Trust tab
> labels every simulation as such inside the app.

## The idea

Loneliness is the problem. Most social apps optimize for engagement or dating.
Haven optimizes for real connection between people who would actually get along,
and treats predatory behavior as a first-class threat to design against.

Three ideas drive the product:

1. **Match on who you are, not just proximity.** Shared interests and background
   drive the match, shown as a compatibility score.
2. **Make meeting in person easy and safe.** An in-chat map suggests real places
   to meet, with partner venues as the revenue model.
3. **Safety as the core feature.** A three-layer detection system (crisis
   support, fast predatory-pattern detection, and a slow-grooming detector that
   reads patterns across weeks) with a human reviewer on every flag.

## What is in the demo

Five tabs, all interactive:

- **Discover** — swipeable match cards with a hand-built SVG compatibility
  graphic, wave-to-connect, local vs. everywhere toggle.
- **Chats** — DMs and interest-based group channels, with stickers, photos,
  simulated voice calls, and an in-chat meetup planner.
- **Map** — a custom pannable SVG map with partner venues, points of interest,
  save-a-spot, and search. No map library, drawn and wired from scratch.
- **You** — editable profile, a private daily mood check-in that redraws an SVG
  mood chart, a journal, and a therapist-export concept.
- **Trust** — the safety system, with two live simulations of the detectors
  catching a fast predatory approach and a slow grooming pattern.

## Built with

Plain HTML, CSS, and vanilla JavaScript. No framework, no build step, no
dependencies. Everything (the map, the charts, the compatibility graphic, the
message photos) is hand-drawn SVG generated in code. Fonts are Google Fonts
(Fraunces + Inter).

The point of building it this way: the entire product is one file a reviewer can
open, read, and run in a browser with nothing installed.

## The business (from the pitch)

A three-pipeline revenue model. B2B2C seat licenses are the main line: a single
10,000-seat employer contract at $4 per seat per month is $480K ARR. A consumer
upgrade tier and per-check-in venue fees layer on top. The pitch modeled a path
from $3.2M ARR in year one to $16.2M by year three, with pilots aimed at
university counseling centers, corporate wellness, and Medicare Advantage.

## Running it

Open `index.html` in any modern browser. That is the whole setup. Or visit the
live demo linked above.
