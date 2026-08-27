# Smash the Quiet — NY Brunch

Working notes for the tennis deck. Source assets pulled from the shared Drive
folder (Colorful Ones / Postcard / Edits), 2026-08-24.

## How this deck relates to the London one

`index.html` is the London deck at the repo root, copied verbatim, with only the
words and the graphics changed. Same CSS, same nine concepts, same animations,
same palette, same timing. If you diff the two files, everything that differs is
either a string or an asset path — plus one appended media query for phones.

That means: no product photography. The original grounds every concept in flat
brand colour, so there is nowhere for the shoot to sit. `assets/` is kept as
source material (the opener's hero was cut from one of those frames) but the
deck does not load it.

**Graphics that were swapped**

| London | NY Brunch |
|---|---|
| `nancy-cream.png` wordmark | `art/logo-cream.png` |
| `truck-cut.png` | `art/smash-ace-hero.png` — Smash and Ace, cut from the shoot |
| `pin-robe/daisy/crown.png` | `art/ball-green.svg`, `ball-pink.svg`, `ball-green2.svg` |
| inline lemon mascot SVG | inline tennis-ball SVG, same viewBox and same face |
| 🍋 🫐 🥑 in the rain | 🎾 |

**Two deliberate departures**, both invisible on a desktop projector:

- Fonts are self-hosted rather than pulled from Google Fonts. Same two faces —
  the deck runs at a venue with no reliable network, and a silent fallback to
  Georgia would be a visibly worse deck with no warning.
- A media query retunes sizes for portrait phones. The layout is unchanged; the
  constants are. It also disables the glitch concept's duplicate-layer effect on
  narrow screens, where the duplicates wrap differently from the real text and
  smear it unreadable. Desktop keeps the original effect exactly.

## Products

**Ace** is the ball — pink and optic yellow. **Smash** is the sage wand.
Get these the right way round: a frame showing only balls is Ace, not "Smash & Ace".
Both read as tennis equipment at a glance, which is the whole gag.

## Four visual worlds in the supplied assets

1. **Product photography** (46 frames in Drive `Edits/`, 28 curated here — 23 landscape,
   5 portrait) — editorial, generous negative space. Four sub-looks: painted court
   corners, pink studio seamless, court flatlays, and net/racket detail. The landscape
   frames full-bleed on a 16:9 projector; the portrait ones are shown as cards.
2. **Campaign hero** — photoreal court, textured ball, multicolour ribbon swoosh
   (`hero-chartreuse.jpg`, `hero-pink.jpg`)
3. **Product on court** — wand with ball head, ribbon trail (`product-court.jpg`)
4. **Mascot / kawaii** — painted ball characters, palm-lined court, sticker outlines
   (`mascot-duo.jpg`, `mascot-trio.jpg`, `mascot-hero.jpg`)

## Known constraints

- **The campaign and mascot art is portrait** (4:5 — 1632×2048 and 1080×1350) against a
  16:9 projector. Full-bleed use would crop away the composition, so those are staged as
  framed elements with extended grounds. The product photography is landscape (3:2) and
  full-bleeds cleanly.
- Assets here are optimised for projector playback (JPEG, max 2560px landscape / 2048px
  portrait). Originals stay in Drive.
