# TYPOGRAPHY-STUDIES.md
### Four pairings, evaluated on editorial authority, cultural seriousness, contemporary restraint, Spanish diacritics, web performance, and licensing reality — then a selection.

*Principle: type does the heavy lifting that boxes did in v1. Hierarchy comes from scale, weight, and space — not containers. Every face must render `á é í ó ú ñ ü ¡ ¿` cleanly at all sizes, because Spanish is a peer, not an afterthought.*

---

## Pairing 1 — Fraunces (display) + Inter (text/UI)
- **Display:** *Fraunces* — a variable "old-style" serif with high contrast, optical sizing, and real character (soft/wonk axes). Lyrical and human at large sizes — the "song."
- **Text/UI:** *Inter* — a neutral, hyper-legible grotesque; excellent for facts, labels, indices, and dense Spanish.
- **Diacritics:** Both have complete, well-drawn Latin-Extended coverage; accents and ñ are crisp.
- **Performance:** Both free (OFL), on Google Fonts, variable — subset to Latin-Extended, self-host in production; small footprint.
- **Licensing reality:** Free for web/commercial. Zero risk. Ships today.
- **Read:** Editorial and warm without being fashion-y; the serif carries emotion, the grotesque carries information. Strong for the archive concept.
- **Risk:** Inter is common — but as the *quiet* voice that's a feature, not a liability.

## Pairing 2 — GT Sectra (display) + Söhne (text) — *premium tier*
- **Display:** *GT Sectra* — a contemporary serif with a "scalpel/calligraphic" edge; serious, cultural, distinctive.
- **Text:** *Söhne* — a refined neo-grotesque (Akzidenz lineage) with quiet authority.
- **Diacritics:** Both excellent, professionally hinted.
- **Performance:** Good, but must be licensed and self-hosted.
- **Licensing reality:** **Paid** (Grilli Type + Klim). Real per-domain/webfont fees. Best-in-class result; requires budget and a license the org owns.
- **Read:** The most "institution-grade" of the four — museum/editorial credibility.
- **Risk:** Cost + procurement; overkill if budget is thin. Recommended *aspirational* target.

## Pairing 3 — Newsreader (display + text) + IBM Plex Mono (index)
- **Display/Text:** *Newsreader* — a variable serif built for on-screen reading with a newspaper heritage and true italics; sets the whole page in one warm archival voice.
- **Index/labels:** *IBM Plex Mono* — for tracked-out section numbers, dates, metadata ("01 — EL SON").
- **Diacritics:** Full, careful Latin-Extended; italics handle Spanish beautifully.
- **Performance:** All free (OFL), variable; light.
- **Licensing reality:** Free. Zero risk.
- **Read:** The most literally "archival/editorial" — one serif family top to bottom = a printed-program feel. Mono adds a contemporary, catalog-index counterpoint.
- **Risk:** Serif-only body can tire on very dense screens; the mono must be used sparingly or it reads "techy."

## Pairing 4 — Canela (display) + Neue Haas Grotesk (text) — *premium tier*
- **Display:** *Canela* — a serif/sans hybrid with high glamour; large-size drama.
- **Text:** *Neue Haas Grotesk* — the definitive quiet grotesque.
- **Diacritics:** Excellent.
- **Licensing reality:** **Paid** (Commercial Type + Linotype). Beautiful but expensive; Canela leans *fashion*, which the brief warns against.
- **Read:** Gorgeous but risks the "make it look like a fashion brand" failure mode.
- **Risk:** Cultural-warmth deficit; cost. Not recommended for this subject.

---

## Selection

**Ship now: Pairing 1 — Fraunces + Inter.** **Aspirational upgrade: Pairing 2 — GT Sectra + Söhne** (if the org will license and own the fonts).

**Why Pairing 1 for the prototype and launch.**
- **Editorial authority + warmth:** Fraunces at display scale is characterful and human (the "song"); Inter is invisible in the best way for facts and Spanish density.
- **Spanish is safe:** both have complete, well-drawn diacritics — no fallback boxes, no clumsy accents.
- **Licensing reality:** free, self-hostable, ships tonight with zero procurement — honest about budget for a nonprofit running a deficit year.
- **Performance:** variable fonts, Latin-Extended subset, self-hosted → fast on mobile (a core-audience requirement).
- **It fits the concept and palette:** a lyrical serif + quiet grotesque on warm paper *is* a contemporary archive.

**Type system rules (replacing boxes as the hierarchy engine):**
- **Display (Fraunces):** section openers and emotional lines set very large (clamp up to ~7–9vw), tight leading, generous margins. Scale = importance.
- **Index labels (Inter, tracked +0.18em, uppercase, silver):** "01 — EL SON," "AHORA," dates, credits — these replace chips/eyebrows.
- **Body (Inter):** 1–1.15rem, generous measure (~62ch), `--ink-soft`.
- **Pull-quotes (Fraunces italic):** used as "voice."
- **Numerals:** tabular for prices/years/stats.
- **Bilingual:** components sized to the *longer* Spanish string; `lang` set correctly; never text baked into images.
- **Oxblood** appears in type only as a rare inline emphasis or link underline — never as a headline fill.
