---
name: PitchPoint
description: Contract business development, told as one gold point reorganising a navy field of contacts.
colors:
  navy: "#13151d"
  navy-2: "#1b1e29"
  navy-line: "#2a2e3c"
  smoke: "#f1ece7"
  smoke-dim: "#c9c3bc"
  smoke-mute: "#a39e98"
  smoke-rule: "#d6cfc6"
  gold: "#a4946f"
  gold-hi: "#c9b68a"
  gold-ink: "#6c5f40"
  ink-soft: "#3e414b"
typography:
  display:
    fontFamily: "DM Sans, system-ui, sans-serif"
    fontSize: "clamp(2.6rem, 5.3vw, 5.1rem)"
    fontWeight: 700
    lineHeight: 1.02
    letterSpacing: "-0.035em"
  figure:
    fontFamily: "DM Sans, system-ui, sans-serif"
    fontSize: "clamp(4.5rem, 10vw, 8.5rem)"
    fontWeight: 700
    lineHeight: 0.85
    letterSpacing: "-0.06em"
  headline:
    fontFamily: "DM Sans, system-ui, sans-serif"
    fontSize: "clamp(2.3rem, 4.3vw, 3.9rem)"
    fontWeight: 700
    lineHeight: 1.04
    letterSpacing: "-0.035em"
  title:
    fontFamily: "DM Sans, system-ui, sans-serif"
    fontSize: "1.06rem"
    fontWeight: 600
    lineHeight: 1.25
    letterSpacing: "-0.01em"
  body:
    fontFamily: "DM Sans, system-ui, sans-serif"
    fontSize: "1.0625rem"
    fontWeight: 300
    lineHeight: 1.65
  lead:
    fontFamily: "DM Sans, system-ui, sans-serif"
    fontSize: "1.18rem"
    fontWeight: 400
    lineHeight: 1.5
  label:
    fontFamily: "DM Sans, system-ui, sans-serif"
    fontSize: "0.72rem"
    fontWeight: 500
    lineHeight: 1
    letterSpacing: "0.14em"
  action:
    fontFamily: "DM Sans, system-ui, sans-serif"
    fontSize: "0.8rem"
    fontWeight: 600
    lineHeight: 1
    letterSpacing: "0.1em"
rounded:
  none: "0px"
spacing:
  gutter: "clamp(1rem, 4vw, 3.5rem)"
  stack-sm: "1.1rem"
  stack-md: "1.6rem"
  stack-lg: "2.2rem"
  section: "clamp(5rem, 12vh, 9rem)"
components:
  button-primary:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.navy}"
    typography: "{typography.action}"
    rounded: "{rounded.none}"
    padding: "1rem 1.35rem"
  button-primary-hover:
    backgroundColor: "{colors.gold-hi}"
    textColor: "{colors.navy}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.smoke}"
    typography: "{typography.action}"
    rounded: "{rounded.none}"
    padding: "1rem 1.35rem"
  button-ghost-hover:
    backgroundColor: "{colors.smoke}"
    textColor: "{colors.navy}"
  text-link:
    textColor: "{colors.smoke}"
    typography: "{typography.action}"
    padding: "1rem 0.25rem"
  nav-link:
    textColor: "{colors.smoke}"
    typography: "{typography.action}"
    padding: "0.5rem 0"
  service-row:
    textColor: "{colors.smoke-mute}"
    typography: "{typography.title}"
    padding: "1.05rem 0"
  index-column:
    backgroundColor: "{colors.smoke}"
    textColor: "{colors.navy}"
    padding: "2rem 2rem 2.5rem 2rem"
---

# Design System: PitchPoint

## Overview

**Creative North Star: "The Point"**

One gold point moves through a deep navy field of smoke-coloured contacts and reorganises it. The whole system is built around that single act: a dark, quiet ground, thousands of small pale dots, and gold reserved for whatever PitchPoint is doing right now (the point, the line it draws, the action you can take). Type is the brand's own: DM Sans Bold in sentence case, set large and tightly tracked, over DM Sans Light body (standing in for the live site's Corp Light). It states one thing per chapter and then gets out of the way.

The page is a scroll story, not a stack of sections. A fixed full-bleed WebGL particle field sits behind everything and morphs, chapter by chapter, between built forms (scattered field, isolated silos, a dinner table for sixteen, an Asia Pacific globe, a fanned document deck, broadcast rings, a pipeline over terrain, a data hall with turbines, carbon strata, and finally the six-spoke asterisk). Copy blocks float over it on a soft navy vignette. After the story, one warm smoke "index" panel lists every service in plain columns, then a navy footer hands over the email address at display size.

Density is low and deliberate: each chapter holds a headline, one or two paragraphs and at most three service rows. Corners are square, controls are hairline-bordered, and depth comes from light (additive particles, a gold glow sprite) rather than from shadows or cards.

**Key Characteristics:**
- Navy ground, smoke text, gold only for the point, its lines and actions.
- DM Sans 700 sentence-case display with tight tracking; DM Sans 300 body; small tracked uppercase labels.
- Six-spoke asterisk as the only marker: list bullets, dividers, active rail state, the final 3D form.
- Square corners everywhere; 1px hairline rules and borders.
- A scroll-scrubbed 3D stage system with a choreographed camera per chapter.

## Colors

A two-temperature palette: cold deep navy and warm smoke, with a muted brass gold as the single accent.

### Primary
- **Brass Point Gold** (`gold`): primary button fill and border, asterisk markers, the scroll meter, list bullets, selection highlight. On light surfaces it is only ever a mark, never text.
- **Lit Gold** (`gold-hi`): hover state of gold fills, the `em` accent phrase inside headlines, active rail item, focus ring, and the WebGL accent colour for particles, glow and lines.
- **Ink Gold** (`gold-ink`): the darkened gold used for small labels on the smoke panel, where `gold` would fail contrast.

### Neutral
- **Deep Navy** (`navy`): page and WebGL clear colour, footer, text on gold buttons, ink on the light panel.
- **Navy Raised** (`navy-2`): reserved second ground tone; not used by the current build.
- **Navy Hairline** (`navy-line`): 1px rules between service rows, deliverable lines, footer base rule, scrollbar thumb.
- **Warm Smoke** (`smoke`): primary text on navy, the light index panel background, the base particle colour.
- **Smoke Dim** (`smoke-dim`): body paragraphs and focus-area list on navy.
- **Smoke Mute** (`smoke-mute`): secondary copy, rail labels, footer column headings, meta lines.
- **Smoke Rule** (`smoke-rule`): 1px dividers on the light panel (column separators, area and client rules). Currently a literal in the CSS, not a custom property.
- **Ink Soft** (`ink-soft`): body copy on the smoke panel.

### Named Rules
**The Point Rule.** Gold marks where PitchPoint is acting: the glowing point, the line it draws, the asterisk, the call to action, the one emphasised phrase per headline. It never fills large areas and never becomes a background.

**The Two Grounds Rule.** There are exactly two surfaces: navy (the story, the footer) and smoke (the index panel). The header inverts to smoke-on-ink when it crosses the smoke panel, rather than introducing a third tone.

## Typography

**Display Font:** DM Sans 700, the live site's own heading face (self-hosted variable file, 300 to 700). Bison appears only inside the outlined wordmark SVG and is not set as type.
**Body Font:** DM Sans 300, standing in for the live site's Corp Light, with system-ui fallback.

**Character:** One geometric family doing everything: heavy and tight for statements, light and open for explanation, small tracked caps for labels. The condensed Bison voice lives only in the wordmark.

### Hierarchy
- **Display** (700, clamp(2.6rem, 5.3vw, 5.1rem), 1.02, -0.035em): the hero H1 only; on phones clamp(2.2rem, 10vw, 3.1rem). Balanced wrap, sentence case.
- **Figure** (700, clamp(4.5rem, 10vw, 8.5rem), 0.85, -0.06em): a single real number in a work chapter ("182 km"), with the unit at 0.28em in Lit Gold.
- **Headline** (700, clamp(2.3rem, 4.3vw, 3.9rem), 1.04): chapter H2s. The light panel and Connect raise it to clamp(2.8rem, 6vw, 5.2rem).
- **Title** (600, 1.05 to 1.06rem, -0.01em, sentence case): service names and index terms; column H3s run clamp(1.45rem, 2vw, 1.8rem) at 700.
- **Body** (300, 1.0625rem / 1rem on phones, 1.65): paragraphs, max 62ch. **Lead** (400, 1.18rem, 1.5) opens a chapter in full Smoke.
- **Label** (DM Sans 500, 0.62 to 0.8rem, 0.12 to 0.16em tracking, uppercase): rail, focus areas, deliverable lines, hours, footer headings, scroll cue, scene annotations, cursor hint.
- **Action** (DM Sans 600, 0.8rem / 0.76rem in nav, 0.1em, uppercase): every button, nav link and text link.

### Named Rules
**The One Phrase Rule.** Each headline carries at most one Lit Gold phrase, set as non-italic `em` (font-style normal). It is the turn of the sentence, not decoration.

**The Display Ceiling Rule.** Display type caps at 5.2rem, the figure numeral at 8.5rem. Display tracking stays between -0.035em and -0.06em; it never goes uppercase.

## Layout

A single full-width column with a fluid gutter (`spacing.gutter`). Story chapters are at least 140vh tall (150vh on phones) so the 3D morph has room to scrub; the hero and Connect are 100svh. Copy sits left by default and alternates to the right (`.right`, with up to 6rem extra inset) so the 3D form occupies the opposite half; the camera's screen-shift offset is choreographed to match that side. Copy width is min(31rem, 40vw) on desktop, min(34rem, 58vw) below 1000px, full width below 760px, where copy anchors to the bottom of the viewport over a bottom-up navy gradient.

The smoke index panel uses a 1.1fr / 1fr heading row and a three-column grid of services with 2rem column padding and a 2px ink top rule; it collapses to one column below 1000px. The footer grid is 1.4fr + 1fr + 1fr, then 2 columns, then 1.

Breakpoints are 1000px (rail and scroll cue hide, grids collapse) and 760px (nav text links hide except Connect, copy moves to bottom, lower particle count). Vertical rhythm steps in roughly 1.1rem, 1.6rem and 2.2rem between copy elements.

## Elevation & Depth

The interface layer is flat: no cards, no resting shadows. Depth belongs to the WebGL stage behind it. Particles are drawn with additive blending, fade with camera distance (6 to 48 units), and brighten toward gold where they carry accent; the gold point is a radial-gradient sprite with a pulsing halo. Copy legibility over the field comes from a soft radial navy vignette behind each copy block (rgba(19,21,29) at 0.95 to 0), and the fixed header uses a navy-to-transparent gradient (smoke-to-transparent over the light panel).

### Shadow Vocabulary
- **Gold lift** (`box-shadow: 0 10px 30px -12px rgba(164,148,111,.7)`): primary button hover only. Ghost buttons drop it.

### Named Rules
**The Light Not Shadow Rule.** Depth is made with light on navy (additive glow, distance fade, vignettes), never with drop shadows on panels.

## Shapes

Square corners throughout (0px): buttons, rail chips, scrollbar thumb, rail dots (4px squares). Lines are 1px hairlines (2px for the ink rule that opens the services grid and for the top scroll meter). The six-spoke asterisk (`assets/asterisk.svg`, also inlined as a symbol and a CSS mask) is the one recurring silhouette: 11 to 16px as a marker, rotating slowly (9s) on the active rail item, and rebuilt from particles as the final 3D form. Arrow glyphs are stroked SVG with square caps.

## Components

### Buttons
- **Shape:** square (0px), 1px border in the fill colour.
- **Primary:** Brass Point Gold fill, navy Action type, 1rem 1.35rem padding, trailing 14px arrow.
- **Hover / Focus:** fill and border shift to Lit Gold with the gold lift shadow, arrow nudges 4px right; 0.4s on the shared ease. Focus is a 2px Lit Gold outline at 4px offset.
- **Ghost:** transparent with a currentColor 1px border; hover fills Smoke with navy text (Ink with Smoke text on light surfaces). Used for the header Connect and the phone call action.

### Text link
Action type with a trailing down arrow, no underline, arrow drops 3px on hover. Used as the secondary hero action.

### Navigation
Fixed header: wordmark (118 to 150px, currentColor) left, nav right. Nav links are Action type at 0.9rem with a 1px underline that wipes in from the left on hover. Below 760px only the ghost Connect button remains. The header colour inverts over the smoke panel.

### Chapter rail
Fixed right-centre ordered list of chapters: label type in Smoke Mute with a 4px square dot. On hover or active, a navy chip label slides in; the active item turns Lit Gold and its dot becomes a spinning asterisk. Hidden below 1000px and once the smoke panel is reached. A 2px gold scroll meter runs across the top.

### Service rows
A list ruled top and bottom with Navy Hairline, each row a 1.1rem asterisk column plus a Title name in Smoke and a one-line description in Smoke Mute. Max three per chapter.

### Deliverable line
Label type in Smoke Mute under a Navy Hairline top rule: "Client · Deliverable". Closes each work chapter.

### Index columns (light panel)
Smoke ground, ink type. Column H3s carry a gold asterisk; terms are uppercase Title, definitions DM Sans in Ink Soft. Columns divide with 1px Smoke Rule.

### 3D stage system (signature)
One Three.js `Points` cloud (12,000 particles, 6,500 on phones) is assigned a target layout per chapter by a seeded `Stage` builder; unused particles fill as ambient dust. Each particle carries position, accent (0 smoke to 1 gold) and size. Scroll position maps to a fractional stage index via chapter centres; the cloud eases toward it (exponential, rate 5.5) and morphs between adjacent stages with smoothstep and a sinusoidal swirl so transitions read as gathering. A per-chapter camera shot (position, target, screen-shift) interpolates alongside. Gold `Line` geometry draws progressively for the pipeline and Adelaide-to-Asia arcs. The gold point sprite follows a per-chapter anchor (cursor-led in the hero). The cursor pushes particles aside in a halo and tints them gold. On load every particle is released from the gold point in a staggered burst (2.8s) while the camera pulls in. The cursor parts the field in a halo that widens with pointer speed and tints dots gold; a click sends a gold shockwave ring outward through the field. The point leaves a short fading wake. Particles carry a depth-of-field blur: dots away from the camera's focal distance grow and soften with area-compensated alpha.

Post-processing runs as one chain: render, UnrealBloom (strength 0.6, radius 0.5, threshold 0.22), output, then a lens pass with radial chromatic aberration, a slight barrel squeeze and a camera FOV kick that all scale with scroll speed, a vignette and fine grain (0.03). Colour management is off (linear output) so the navy ground and faint dust stay exactly as authored.

Scene annotations: per-chapter labels are pinned to 3D anchors and projected each frame (gold diamond, hairline leader, navy chip with a clip-path wipe). They flip side to stay in the viewport, and the pipeline tip counts its live distance in km. Reduced motion freezes time-based animation; no WebGL hides the canvas and leaves the copy intact.

### Photography (their own library)
PitchPoint's photographs and deliverable shots live in `assets/photos/`, resized from the live site's library (pitchpoint.com.au CDN). They appear two ways:
- **In the 3D story**, as plates set behind the particles: one or two per chapter (dinners for the room, the Asia Pacific aerial, the InDeMa capability statement, communications, the Bowen pipeline site, the turbine at dawn and the data centre for TBH, the CO2CRC prospectus). Plates are placed in screen space on the side opposite the copy, so they always land in frame. At rest each one is printed as a navy/smoke duotone with gold mid-tones, framed by a gold hairline, and it dissolves in along a gold burn line as its chapter arrives. Hovering turns it full colour and brings it forward, and the cursor hint reads "Full colour". Particles draw over the plates with additive light. Captions are short Label-type lines under the plate, hidden on phones.
- **On the smoke panel**, as "Made for the room": a drag-to-browse strip of real client collateral (InDeMa, CO2CRC, Bunnings Trade, Bowen, Energy Australia, and a legal seminar). Each caption gives the client and the deliverable as printed on the document. The function & campaign planner gets a resource block with a mailto request.

**The Real Pictures Rule.** Only PitchPoint's own photographs and deliverables are used, and captions say only what the image or the live site states. No stock imagery is added and no client is inferred.

### Motion
One easing for everything: `cubic-bezier(.16,1,.3,1)`. Headlines rise word by word out of a clipped line (112% to 0 with a 4deg tilt, 38ms stagger; the hero waits 1.1s for the intro). Other copy children fade up 28px from a 6px blur over 1.1s. Buttons and text links lean toward the cursor (magnetic, 0.22 to 0.35 of the offset). Hover transitions run 0.4 to 0.6s. Reduced motion removes animation, grain and lens response.

## Do's and Don'ts

### Do:
- **Do** keep gold to the point, its lines, the asterisk, actions and one headline phrase (The Point Rule).
- **Do** set headlines in DM Sans 700 sentence case with tight tracking; keep uppercase for small tracked labels and actions only.
- **Do** use the six-spoke asterisk as the bullet, divider and active marker; draw it from the shipped SVG.
- **Do** keep corners square and borders 1px; use `navy-line` on navy and `smoke-rule` on smoke.
- **Do** use `gold-ink`, not `gold`, for small text on the smoke panel.
- **Do** give every new chapter a 3D stage and a camera shot, with copy on the side opposite the form.

### Don't:
- **Don't** introduce rounded corners, cards or resting drop shadows on the navy story.
- **Don't** add a third surface tone; navy and smoke are the only grounds.
- **Don't** use more than one gold phrase in a headline, or italicise it.
- **Don't** add statistics, testimonials or figures the work did not produce; the figure style is for one real number.
- **Don't** add a second easing curve.
