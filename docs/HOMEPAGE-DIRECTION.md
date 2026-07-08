# HOMEPAGE-DIRECTION.md
### The permanent homepage — a directed sequence
*Concept: "El son que no termina / The song that doesn't end." Palette: Archival Editorial (paper/ink/silver + oxblood ~2%). Type: Fraunces + Inter. The homepage is the institution; the 2026 concert is its current chapter, entering only when it has earned meaning.*

**Direction discipline:** the visitor should feel a hand deciding what they see first, what is withheld, when information arrives, when the page goes quiet, when it surges. No cards, no tiles, no chips. Hierarchy is scale, space, sequence, and full-bleed media. Every "image" below is a **placeholder film-frame** in the prototype (no licensed photography) and is captioned as such.

---

### 00 — Masthead (near-invisible)
Thin, paper-colored, no border. Wordmark left (Fraunces), five words of nav, `[ES]`, and one quiet **Tickets** link (oxblood underline). It should almost disappear over the opening frame.

### 01 — OPENING · the song (cultural statement, not an event)
- **What.** A single full-bleed frame — human detail: a breath before the trumpet, hands on the vihuela, embroidery catching light, dusk over the Bowl. Almost no UI. One line, set very large in Fraunces, arriving *after* the image lands.
- **Copy (draft).** *"For twenty-nine years, the song hasn't stopped."* / ES: *"Desde hace veintinueve años, el son no se detiene."* Sub, small, silver index: `SANTA BARBARA MARIACHI FESTIVAL · EST. 1996`.
- **No** ticket price, no seat tiers, no poster. This is a statement.
- **Motion.** Image holds; the line fades up once (600ms); a faint scroll cue. Reduced-motion: static.
- **Mobile.** Full-height frame, the line reflowed to 2–3 lines, still dominant.

### 02 — THE CURRENT MOMENT · this year's verse
- **What.** The page breathes to paper. Now — and only now — the current edition enters, quietly and confidently, as *this year's verse of the ongoing song*.
- **Copy.** Index: `AHORA / NOW`. Display: **"This year, the 29th verse."** Line: *29th Annual Santa Barbara Mariachi Festival · Saturday, August 8, 2026 · Santa Barbara Bowl.* One text link: **Enter the 2026 festival →** (to `/2026`).
- **Composition.** Asymmetric: a large left-aligned Fraunces statement, a narrow right column of facts in Inter, wide negative space between. No box around the date.
- **Motion.** Type reveals in reading order; a hairline rule "draws" left-to-right. Mobile: stacked, generous spacing.

### 03 — THE MUSIC · living art, full-bleed
- **What.** Mariachi as discipline, heritage, and present-tense craft. A full-bleed sequence (2–3 frames) with large editorial captions floating in the margins — never captions-in-a-card.
- **Copy (draft).** *"Not a costume. A discipline."* / *"Brass, strings, and a cry that carries."* Short body in the margin about the form and the festival's stewardship. Link: **The music →** (`/the-music`).
- **Motion.** Slow horizontal drift on one frame (parallax ≤15%); captions fade in the negative space. Mobile: vertical frames, captions below, still full-bleed.

### 04 — THIS YEAR'S VOICES · artists as cinematic chapters
- **What.** The current lineup — **not** three equal tiles. Each artist is a *chapter*: a near-full-viewport frame where the artist dominates, name set huge in Fraunces overlapping the image edge, one line of context, a quiet link. Scroll (or horizontal film-strip on wide screens) moves to the next.
- **Copy per artist.** Name (display), role/index (`HEADLINER / CABEZA DE CARTEL`, `INVITADO`, etc.), one sentence, **Listen →** and **See them Aug 8 →**.
- **Working 2026 data (client-side, replaceable):** Majo Aguilar · Joss Favela · Mariachi Los Camperos · + more to confirm. Rendered from the edition data object so any year swaps cleanly.
- **Composition.** Layered portraits, type interacting with image, controlled overlap; one dominates the viewport at a time. No grid of equals.
- **Motion.** Cross-dissolve/reveal between artist chapters; name settles as the frame arrives. Mobile: one artist per full screen, swipe/scroll; type still large.

### 05 — THE REASON · scholarship as the song carried forward (major reveal)
- **What.** The emotional turn. The visitor realizes the night funds something beyond the stage — and that *this is how the song continues*: tonight's audience sends local students forward. Handoff framing (T2): a recipient's face and words.
- **Copy (draft).** *"The concert lasts one night. What it pays for lasts a lifetime."* / ES: *"El concierto dura una noche. Lo que financia dura toda la vida."* Then, human and specific: a recipient portrait, first-person pull-quote (Fraunces italic), destination college. Stat, set as type not a badge: *Since 1996 — [reconcile figure] in scholarships for local Latino students.* Link: **Scholarships →**.
- **Composition.** Full-bleed portrait, quote in the margin, one oxblood downbeat mark. No stat "cards."
- **Motion.** The portrait holds; the quote arrives line by line; the number sets once (count-up only if reduced-motion is off). Mobile: portrait full-screen, quote beneath.

### 06 — LEGACY · the long song (archive becoming present)
- **What.** 1996 → 2026 as continuum. No timeline cards. A single archival frame *becomes* a present-day frame (same-stage dissolve) as the year advances with scroll; a quiet waveform/year-rail runs beneath.
- **Copy.** *"One long song, in twenty-nine verses."* Index years as the rail: `1996 … 2006 … 2016 … 2026`. Link: **Explore the archive →** (`/legacy`).
- **Motion.** Scroll-driven crossfade at the emotional peak (echo accent from T3); native scroll only. Mobile: two-frame dissolve, rail as a slim progress line.

### 07 — STORIES · the people who carry it (editorial, not cards)
- **What.** Recipients, artists, families, community — as *editorial features*, not quote cards. One large lead story (full-bleed image + headline in the margin) and two quieter text-led entries beneath, separated by space and rule, not borders.
- **Copy.** Feature headline + dek in Fraunces/Inter; **Read →**. (Uses real names/colleges only with consent; placeholders flagged.)
- **Motion.** Lead image parallax; entries fade in. Mobile: stacked, generous whitespace.

### 08 — RETURN TO THE VERSE · the current-festival CTA, now earned
- **What.** Only here does the site ask for the sale — and now it *means* something, because the visitor understands the mission. A calm, confident full-width paper section.
- **Copy.** *"Take your seat in the song."* / ES: *"Toma tu lugar en el son."* Facts line: *Aug 8, 2026 · Santa Barbara Bowl · Gates 4 / Show 5 · from $79.* Primary: **Get tickets** (oxblood; → `/2026/tickets`). Secondary: **Plan your night**.
- **Motion.** Minimal — the CTA is the payoff, not a spectacle. Mobile: sticky **Tickets** bar may appear from here down (not before), so the ask follows the meaning.

### 09 — PARTNERS · restrained, editorial
- **What.** Sponsors as a *typographic honor roll*, not a logo grid or chips: names set in Inter at readable scale, grouped by tier with quiet labels, plenty of space. A single line thanks the community.
- **Copy.** *"Made possible by Santa Barbara."* Link: **Become a partner →**.
- **Motion.** None beyond a soft fade. Mobile: single column list, not a wall.

### 10 — CLOSING · a permanent close, then the ask
- **What.** An institutional close that would read well any month of the year, then one final quiet CTA and capture.
- **Copy.** *"The song doesn't end. It waits for the next verse."* / ES: *"El son no termina. Espera el siguiente verso."* Capture: *Be first to hear the 2026 lineup.* Footer: 501(c)(3), EIN 77-0472982, correct email, address, `[ES]`, social — organized, calm, no chips.
- **Motion.** Still. The page ends on breath, not fireworks.

---

## Scroll logic
Statement (01) → the institution places the year (02) → the art (03) → this year's voices (04) → **the reason** (05, the turn) → the long song (06) → the people (07) → **now buy, with meaning** (08) → partners (09) → permanent close (10).
Conversion is *withheld* until it has been earned — the opposite of v1, which led with price. Yet the sale is never hard to reach: **Tickets** sits in the masthead throughout, and the sticky mobile bar appears from section 08. The homepage sells by making you *care*, then routes all the conversion machinery to `/2026`.
