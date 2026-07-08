# MEDIA-MAP.md
### Media-first homepage — asset inventory, roles, and replacement plan
*Source folder `~/Downloads/Mariachifestival` is treated as READ-ONLY. All originals preserved. Selected assets were **copied** (never moved/renamed/edited in place) into `/public/media/…`. **Every asset here is temporary AI-generated concept media** and must be replaced with real, licensed festival photography/footage before anything ships. **AI-generated people are placeholders only — none may be labeled as Majo Aguilar, Joss Favela, a member of Mariachi Los Camperos, or as a real scholarship recipient.***

## Source specs (all 14 originals)
- **12 stills:** all **1344×768 (16:9 landscape)**, JPEG, ~130–395 KB. Generators: `lucid-origin` (11), `gpt-image-2` (1).
- **2 videos:** both **1366×768, ~5.9s, 24fps**, MP4, 0.85–1.66 MB. Generator: `hailuo-2`.
- Implication: **no portrait originals exist.** Mobile uses `object-position` art-direction crops of the 16:9 frames (documented per scene), not squashing.

## Contact-sheet review artifacts
`/_review/CONTACT_stills.jpg`, `/_review/CONTACT_video.jpg`, `/_review/frames/…` (internal only).

## Selection, scene mapping, and roles

| Scene | Project file | Source (short) | Type | Desktop role | Mobile crop | Quality | Replace with (real) |
|---|---|---|---|---|---|---|---|
| 01 Hero — "before the note" | `hero/hero-trumpet.mp4` (+ `hero-trumpet-poster.jpg`) | hailuo trumpet close-up | video+poster | Full-viewport muted loop; title over lower-left | center; poster on mobile, autoplay if allowed | **A** vivid red→cobalt, controlled motion | Real trumpet close-up (owned footage), 6–10s, quiet motion, room for type |
| 01 Hero alt / anticipation still | `hero/hero-trumpet-still.jpg` | gpt-image trumpet | image | Reduced-motion + fallback hero; strong dark negative space L | left-weighted | **A** | Same as above (still frame) |
| 02 Detail becomes world | `detail/embroidery.jpg` | silver embroidery macro | image | Masked reveal that scales past viewport | tight macro center | **A** gorgeous texture | Macro of a real charro suit / botonadura |
| 03 Release (performance) | `performance/performance.mp4` (+ `performance-poster.jpg`, `performance-crowd.jpg`) | hailuo live seq / wide-from-behind | video+stills | Energy explosion; muted loop | center; poster still on mobile | **A** cobalt evening + warm | Real festival performance footage at the Bowl |
| 04 Who it belongs to | `people/family-generations.jpg` + `people/child-watching.jpg` | 3 generations / child watching | images | Overlapping human planes in negative space | family: center; child: right-weighted | **A** golden hour / red bokeh | Real documentary family + audience photography (with releases) |
| 05 Now / 2026 — artists | `artists/artist-a.jpg`, `artists/artist-b.jpg`, `artists/ensemble.jpg` | female star / male singer / ensemble | images | Overlapping portrait planes, architectural names | one-at-a-time full-bleed | **A–B** vivid | **REAL licensed artist photos** of the confirmed lineup. **AI faces = placeholders; do NOT name.** |
| 06 Night becomes opportunity | `scholarships/student-future.jpg` | first-gen college student, daylight | image | Bright surprising transition | center, headroom | **A** optimistic daylight | Real, consented scholarship-recipient portrait |
| 07 Time (legacy) | `legacy/legacy-doubleexposure.jpg` | B&W historic ↔ color contemporary | image | Past→present transition anchor | center | **B** (composite look, intentional) | Real archival frame graded → real present frame |
| 08 Return to place (venue) | `venue/bowl-bluehour.jpg` | hillside amphitheater, blue hour | image | Ticket CTA earned here | center, sky headroom | **A** blue hour | Real Santa Barbara Bowl at blue hour (owned/licensed) |
| 09 Finale | `finale/finale-peak.jpg` | ensemble, bows raised, cobalt+red | image | Full-width high-energy close | center | **A** | Real finale/crowd moment at the Bowl |

**Unused originals:** none discarded — S08 kept as `performance-crowd.jpg` (poster/support for the performance video). Every strong asset has a role; nothing was forced.

## Chromatic arc (derived from the actual media, not a fixed palette)
Hero **cobalt+magenta+silver** → detail **red+silver+black** → release **red+cobalt stage** → family **golden daylight** → artists **vivid red/editorial** → scholarship **bright warm daylight** → legacy **mono→color** → venue **blue hour** → finale **cobalt+red night**. The page changes color as you move — film color direction, not one flat palette. UI chrome stays neutral (near-white / true near-black / silver) so the media carries the color.

## Hard rules encoded in the build
- AI artist/person images sit behind a data layer; each has a code comment `REPLACE: real licensed [artist|recipient] photo`. Real assets swap in without redesign.
- No AI image is captioned as a real named person, venue-as-documentary-proof, or real recipient.
- Videos: `muted`, `playsinline`, `loop`, `preload=none`, poster set; paused off-screen; disabled under `prefers-reduced-motion` (poster shown).

## ADDENDUM — Female-singer asset for the 2026 Festival feature (v4+)
- **Project file:** `artists/artist-a.jpg` (source: `lucid-origin_..._young_female_regional_Mexican_music_star...`). A striking editorial image — performer framed by swirling red silk against cool blue sky, silver jewelry.
- **Role:** emotional anchor of the redesigned **2026 Festival feature** (the "major female headliner" moment), standing in for **Majo Aguilar**.
- **HARD RULE — do not misrepresent:** this is an **AI-generated person and is NOT Majo Aguilar.** It must never be captioned as her. It is used only as an *atmospheric* placeholder; the artist **bill** names Majo Aguilar as headliner in a separate typographic zone, and the image carries a visible "concept placeholder" caption. Code comment on every use: `REPLACE: licensed Majo Aguilar campaign photography`.
- **Chromatic value:** vivid carmine/vermilion silk + cobalt sky + silver — anchors the 2026 feature's color and pairs with the trumpet hero.
- **A3 correction (composition, not disclaimer):** the image reads as a **beauty/jewelry campaign**, and placing it beside the name "Majo Aguilar" falsely implies it *is* her. In A3 it is used only as **abstract campaign ATMOSPHERE** (cropped toward the swirling red fabric with the face partial/at the edge), and the **2026 lineup is a separate typographic zone** — the name "Majo Aguilar" is not adjacent to the face. **REPLACE WITH APPROVED / LICENSED MAJO AGUILAR CAMPAIGN MEDIA BEFORE ANY PRESENTATION OR PUBLICATION.** No alternative female *performance* asset exists in the folder (see MISSING-MEDIA Gap 3).
- **Strongest-per-role (confirmed this pass):** hero = `hero/hero-trumpet.mp4` (+still); **female singer / 2026 = `artists/artist-a.jpg`**; scholarship = `scholarships/student-future.jpg`; family/community = `people/family-generations.jpg`; legacy = `legacy/legacy-doubleexposure.jpg`; performance = `performance/performance.mp4` / `performance-crowd.jpg`; venue = `venue/bowl-bluehour.jpg`.
