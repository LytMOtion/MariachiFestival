# PALETTE-STUDIES.md
### Four sophisticated systems, then a selection
*Governing rule (from the reset): photography carries the color; the UI is near-silent. Light-dominant, editorial, one controlled accent. No gold-on-black, no yellow, no electric blue, no flag palette, no gradient-festival look.*

Each study lists exact hex, the role of each tone, expected share of surface, why it belongs to this institution, and its risks.

---

## Study A — Paper / Ink / Silver (warm editorial)
| Token | Hex | Role | ~Use |
|---|---|---|---|
| Paper | `#F4F1EA` | Primary background — warm mineral white | 62% |
| Ink | `#1A1917` | Body + display type; near-black, warm | 22% |
| Silver | `#B9B4A9` | Rules, captions, secondary type, dividers | 9% |
| Newsprint | `#8A8578` | Tertiary text, metadata, indices | 5% |
| Wine (accent) | `#6E1E28` | Rare emphasis: a single word, a live dot, a link underline | ~2% |

**Why it belongs.** Warm paper + carbon ink is the language of *programs, liner notes, and archives* — exactly the register of a 29-year institution. The wine is drawn from the deep red of a charro suit and moños, so the one accent is *culturally real*, not decorative. Photography (brass, embroidery, dusk) supplies all the warmth and saturation.
**Risks.** Warm paper can tip "vintage/rustic" if type is too calligraphic — mitigate with a contemporary grotesque for UI. Wine must stay scarce or it becomes a theme color.

## Study B — California Evening (cool stone)
| Token | Hex | Role | ~Use |
|---|---|---|---|
| Chalk | `#EDEBE6` | Background — cool white | 58% |
| Stone | `#C7C2B8` | Panels, quiet fields, image mats | 12% |
| Coastal grey | `#9A9C99` | Secondary type, rules | 8% |
| Brown-black | `#17150F` | Type, deep footer | 18% |
| Dusk blue-grey (accent) | `#5A6B72` | Extremely rare — a cold highlight, focus states | ~4% |

**Why it belongs.** Evokes the actual Santa Barbara coast at dusk — the light the festival happens in. Cooler and more restrained than A; reads "West-Coast cultural institution."
**Risks.** The dusk blue-grey drifts toward "corporate/coastal-hotel" if overused; cool whites can feel colder/less inviting for a warm cultural subject. Best if photography is generously warm to counterbalance.

## Study C — Archival Editorial (newsprint)
| Token | Hex | Role | ~Use |
|---|---|---|---|
| Off-white | `#F6F4EF` | Background | 60% |
| Newsprint grey | `#D8D4CB` | Image mats, quiet bands, archival frames | 12% |
| Carbon | `#141310` | Type; true editorial black | 20% |
| Silver | `#A6A199` | Captions, indices, metadata, hairlines | 6% |
| Oxblood (accent) | `#5E1A22` | One controlled cultural accent — section markers, live indicator, key link | ~2% |

**Why it belongs.** This is the *archive made contemporary*: newsprint and carbon are the material of 29 years of clippings, programs, and photographs — the festival's real paper trail — but set with modern discipline. The oxblood is the single deep cultural note (charro red, oxidized), used like a conductor's downbeat. It directly serves the "song that doesn't end / archive becoming present" concept: the UI itself looks like a living archive.
**Risks.** Needs genuinely good photography to avoid feeling austere; oxblood must be rationed to a few touchpoints per page.

## Study D — Monochrome + Human Color (photo-led)
| Token | Hex | Role | ~Use |
|---|---|---|---|
| White | `#FBFAF7` | Background | 60% |
| Soft grey | `#C9C6BF` | Rules, mats | 10% |
| Near-black | `#121110` | Type | 26% |
| Accent (single, chosen per campaign) | e.g. `#6E1E28` | One tone, only when needed | ~4% |

**Why it belongs.** The purest expression of the reset's rule: the *interface is monochrome* and lets full-bleed photography carry *all* color. Maximally timeless; the imagery does the emotional work.
**Risks.** Almost entirely dependent on photography quality — with placeholder art it can feel unfinished; the "one accent per campaign" flexibility can erode consistency without governance.

---

## Selection

**Winner: Study C — Archival Editorial, with the oxblood accent — subsuming the discipline of Study D.**

**Why.**
- It is the exact material analog of the chosen concept ("the song that doesn't end / archive becoming present"): the site *looks like a living archive*, warm paper and carbon with one deep cultural downbeat.
- It is decisively **not** v1 — light-dominant, no gold, no dark-luxury cliché — which is the primary brief.
- Warm off-white reads more inviting than Study B's cool chalk for a warm cultural subject, while staying more disciplined than Study A.
- The single oxblood accent is culturally grounded (charro red) yet rationed to ~2%, so color meaning is preserved and never becomes "themed."
- It adopts Study D's governing principle — **photography carries the color** — as a hard rule.

**Final tokens (locked for the prototype):**
```
--paper:      #F6F4EF   /* background */
--paper-2:    #EFEBE2   /* alternate quiet band */
--newsprint:  #D8D4CB   /* image mats, archival frames */
--carbon:     #141310   /* type */
--ink-soft:   #3A362F   /* secondary type */
--silver:     #A6A199   /* captions, hairlines, indices */
--oxblood:    #5E1A22   /* single controlled accent, ~2% */
--oxblood-lo: #7A2A31   /* accent hover only */
```
Dark full-bleed *photography* moments (a night shot, a stage frame) are allowed and encouraged — the *system* stays paper/ink; darkness comes only from images, never from UI chrome. This is how the site stays cinematic without being "dark."

**Accent governance.** Oxblood appears at most a few times per page: the live/"on sale" indicator, one section downbeat mark, key inline links/underlines, and the primary CTA. Never as a fill behind text, never as a gradient, never as a second brand color.
