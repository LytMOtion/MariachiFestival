# TOMORROW-REVIEW.md
### Santa Barbara Mariachi Festival — direction v2, ready for your review
*Internal concept. Nothing published, no one contacted, live site untouched. v1 archived at `/archive/prototype-v1-rejected/`.*

---

## What I changed (the four corrections, answered)

1. **Institution, not a concert.** The site is now two layers: a **permanent institutional homepage** (`index.html`) built around the festival as an ongoing 29-year tradition, and a separate **2026 edition page** (`festival-2026.html`) that carries all the conversion machinery. Cover August 8 with your hand and the homepage still stands — legacy, scholarships, stories, the music. The concert is a *chapter*, not the identity, and it reads correctly in September.
2. **No more boxes.** Cards, tiles, chips, and bordered modules are gone. Hierarchy now comes from **scale, negative space, full-bleed frames, and sequence.** Artists are cinematic chapters in a horizontal film-strip; the scholarship is a full-bleed reveal; sponsors are a typographic honor roll; seat tiers are a guided list separated by hairlines — not a grid of cards.
3. **New palette — paper, not dark-and-gold.** Light **archival editorial** system: warm paper `#F6F4EF`, carbon ink `#141310`, silver, newsprint, and a single controlled **oxblood** `#5E1A22` accent at ~2%. No yellow, no gold-on-black, no flag colors, no gradients-as-decoration. Darkness appears **only inside photography frames**, never in the UI.
4. **Cinematic through direction, not darkness.** The homepage is a *sequence*: a cultural statement first (no price, no poster), then the year enters, then the music, then this year's voices, then the emotional turn to scholarships, then the long song, then the people, and only then — earned — the ask. Motion is restrained and purposeful (reveals, one scroll-driven crossfade), respects `prefers-reduced-motion`, and never compensates for composition.

## Concept selected — and why

**"El son que no termina / The song that doesn't end."** Mariachi is an inherited, generational tradition; the festival is one continuous song across 29 years; each concert is the current verse; scholarships are how the song is literally carried forward (students → future musicians and first-gen graduates). I chose it over four alternatives (see `CONCEPT-TERRITORIES.md`) because it is the only premise that is **permanent by construction**, makes **scholarships structural rather than sentimental**, turns **annual lineup changes into the whole point**, and is **culturally true** to the form. "The handoff" is folded in as the scholarship's human mechanism; "Under the oaks" is reserved for the 2026 page and venue material.

## What to review first (in order)

1. **`index.html`** — open it, scroll slowly, and toggle **Español** (top right). Judge the *sequence and restraint* first, imagining real photography where the toned placeholder frames are.
2. **`festival-2026.html`** — the conversion counterpart. Confirm the institution↔edition split feels right and that seat selection reads honest, not boxy.
3. **`CREATIVE-RESET.md`** — the diagnosis of v1 and the new principles.
4. **`CONCEPT-TERRITORIES.md`**, then **`PALETTE-STUDIES.md`** and **`TYPOGRAPHY-STUDIES.md`** — the reasoning behind the chosen concept, color, and type, with the alternatives.
5. **`NEW-IA.md`**, **`HOMEPAGE-DIRECTION.md`**, **`2026-FESTIVAL-PAGE.md`** — the structural and section-level blueprints the prototypes implement.

## What is still unresolved (my open questions)

- **The brand line.** "The song that doesn't end / El son no termina" is a *territory*, not locked copy. I'd want a native Mexican-Spanish writer to pressure-test the Spanish line before it's final.
- **The horizontal artist film-strip** is the one interaction I'd most want to test on real devices — it's cinematic on desktop but I want to confirm it feels effortless (not a scroll trap) on trackpads and touch. Fallback to vertical full-screen chapters is already built for mobile.
- **How dark the "photography" moments should go.** With real images the hero/reason/legacy frames will carry the drama; the placeholders only approximate it. This judgment can't be finalized until we see actual photography.
- **Depth of the permanent secondary pages** (The Music, Scholarships, Legacy, Stories) — I specified them in the IA but built the homepage + 2026 page as the priority prototypes. Those interior pages are the next build.
- **A visual QA pass in-browser.** I verified structure and script syntax, but could not run a headless browser render in this environment — a real-device look is worth doing before you form a final judgment on pacing.

## Assets that would transform the prototype most (highest impact first)

1. **One hero-grade film/photo** — a mariachi mid-phrase on the Bowl stage at golden hour. This single asset carries the entire opening.
2. **A confident set of documentary artist portraits** for the film-strip (hands, brass, embroidery, faces mid-song) — not press headshots.
3. **One consented recipient portrait + real first-person quote** for the scholarship reveal. This is the emotional hinge of the whole site.
4. **A graded pair of archival↔present Bowl-stage frames** for the legacy crossfade.
5. **A few real seat-view images** (or AXS FanSight) per terrace for the 2026 seat guide.

## What requires client confirmation before anything ships

- **2026 lineup.** I've rendered Majo Aguilar · Joss Favela · Mariachi Los Camperos · +TBA as *working client data* per your instruction. One honest flag remains: public sources (AXS/Bowl) currently name only **Mariachi Los Camperos** ("…and more"), and the festival's own homepage names **Mariachi Vargas de Tecalitlán**. Please confirm the final bill and billing order — the data model swaps it in one place.
- **Scholarship figure.** The reveal shows `[reconcile figure]`. The org states **$1M+**; a 2025 news source said **$650K+**. Confirm the number (or we use qualitative language).
- **Photo/story rights & recipient consent** for any real imagery or named stories (all current imagery is placeholder; all people/quotes are illustrative).
- **Sponsor roster & tiers** (the honor-roll grouping is illustrative).
- **Type licensing** — prototype ships free Fraunces + Inter; the premium upgrade (GT Sectra + Söhne) needs a purchased, org-owned license.

## Honest note on scope

I prioritized the two prototypes the reset hinged on — the **permanent homepage** and the **2026 edition page** — plus the full written system (reset, concepts, palette, type, IA, homepage direction, 2026 spec). The interior institutional pages (The Music, Scholarships, Legacy, Stories) are specified but not yet built; they're the natural next session. If tomorrow's review confirms the direction, that's where I'd go next.
