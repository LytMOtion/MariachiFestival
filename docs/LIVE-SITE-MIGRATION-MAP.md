# LIVE-SITE-MIGRATION-MAP.md
### Complete audit of the live site → redesign migration
*Source: https://www.thesantabarbaramariachifestival.org/ (Squarespace). All first-party pages followed, English + Spanish. Actions: KEEP · IMPROVE · MERGE · RENAME · ARCHIVE · REMOVE-if-justified. Content is preserved; only weak design is discarded.*

## English pages

**Home** — `/`
Purpose: front door + ticket entry. Content: "29 years" line, wedding-photo hero, Vargas/Los Camperos text, exposed AXS link + shortlink. CTA: Spanish "Compra tus entradas" → shortlink. ES equivalent: partial. Issues: placeholder hero, monolingual CTA on EN page, exposed tracking URL, no date/venue above fold. SEO/migration: **critical**. → **IMPROVE (rebuild as institutional homepage).**

**About Us** — `/projects`
Purpose: who/what/why. Content: mission ("preserve mariachi… scholarships for Latino students"), "From 1995 to today," co-founders **Salud Carbajal & Al Pizano (dec.)**, 29 yrs, a **César Chávez quote**, real gallery photos. CTA: none. ES: `/projects-1` ("Nuestra Historia," but says "27 años" — stale). Issues: thin, no history depth, EN/ES year mismatch. → **KEEP + IMPROVE + SPLIT** into **About › Mission** and **About › History**.

**Board of Directors** — `/board`
Purpose: governance/credibility. Content: intro paragraph on volunteer board + mission; **real headshots by Richard Garnica** (also a sponsor). Members (prior audit): Miguel Martinez (Pres.), Perla Navarro Lewis (VP), Erika Aldaz (Treas.), Liz Ruiz (Sec.), +7. CTA: none. ES: `/board-1` ("Mesa Directiva," **outdated hierarchy** — shows Avila as Pres.). Assets: headshot set (rights: Garnica — confirm). Issues: EN/ES contradiction; no bios. → **KEEP + IMPROVE + MERGE under About › Board**; single source of truth to end EN/ES conflict; elegant leadership layout (not generic headshot cards).

**Scholarships** — `/espanol` *(mislabeled slug — an English page living at `/espanol`)*
Purpose: the mission pillar. Content: scholarship purpose, reception photo galleries, "$1,000,000" claim, **26 named 2024 recipients w/ colleges** (on the ES `/espanol-2`). Partner: **Scholarship Foundation of Santa Barbara**. CTA: none/weak. ES: `/espanol-2` ("Becas"). Issues: no eligibility/application/dates, no recipient voice, $ figure conflicts with press ($650K+ vs $1M+), best content stranded on ES page. → **KEEP + IMPROVE + RENAME `/scholarships`**; expand to Program · Eligibility · Impact · Recipient Stories.

**Our Sponsors** — `/our-sponsors`
Purpose: sponsor recognition. Content: **~30 sponsor logos as screenshots** (e.g., Chumash Foundation, Mechanics Bank, American Riviera Bank, Pacific Beverage, Los Agaves, McDonald's). CTA: none. ES: `/our-sponsors-copy`. Assets: logos (need clean SVGs). Issues: screenshot logos hurt polish/SEO/a11y, no tiers. → **KEEP + IMPROVE** (tiered wall, clean logos) under **Sponsorship › Our Sponsors**.

**Become a Sponsor** — `/sponsors`
Purpose: sponsor conversion. Content: **sponsorship package as a screenshot**, "27th/28th Anniversary Sponsor" (stale year). CTA: none (no form). ES: `/become-a-sponsor-copy` (advertises 2025 cycle). Issues: no form, no downloadable deck, image-baked text. → **KEEP + IMPROVE** (why-partner, tiers, benefits, inquiry form, deck PDF) under **Sponsorship › Become a Sponsor**.

**Upcoming Events** — `/calendar`
Purpose: programming. Content: mixed **past + future** events (festival, receptions, Winter Show/Vocal Competition, VIP Sponsor Party Aug 7), some back to 2023; **no ticket link**. CTA: weak. ES: `/eventos` (2025 only, omits 2026). Issues: past shown as upcoming, no hierarchy, stale ES. → **KEEP + RENAME + SPLIT** into **Events › Upcoming** and **Events › Past**.

**2025 Festival Photos** — `/new-page-2`
Purpose: gallery. Content: **~70–90 photos (RG Photography, 2025)**. CTA: none. ES: none. Assets: photo set (rights: RG Photography — confirm). Issues: generic slug, single-year, no archive structure, filename alt text. → **KEEP + RENAME `/gallery`** → **Gallery / Archive** (by edition/year).

**Mariachi Recommendations** — `/new-page-1`
Purpose: **real community directory** — a list of Santa Barbara County mariachis; invites local groups to email to be added. Content: a graphic + instructions to email `mariachifestivalsb@gmail.com`. CTA: email. ES: none. Issues: content is thin/graphic-only, no actual list shown publicly, generic slug. → **KEEP + IMPROVE** under **Community › Mariachi Directory** (only if org maintains the list; otherwise ARCHIVE). Do **not** delete — it's a genuine community function.

**Contact Us** — `/contact`
Purpose: reach org. Content: address, email, socials; "28th Anniversary Sponsor" stale copy; **transposed mailto** (`sbmariachifestival@` vs site's `mariachifestivalsb@`). CTA: email. ES: `/contact-1`. Issues: possibly-bouncing mailto, stale year, "© 2015" seen on some pages. → **KEEP + IMPROVE** (fix email, add form, volunteer/board pathways).

## Spanish pages (parallel, drifting)
`/projects-1` (Nuestra Historia — "27 años"), `/board-1` (Mesa Directiva — outdated board), `/espanol-2` (Becas — has the 26 recipients), `/our-sponsors-copy`, `/become-a-sponsor-copy` (2025 cycle), `/contact-1`, `/eventos` (2025 only). No ES Home, no ES Gallery, **no ES ticket path**. → **MERGE + REBUILD** into a single first-class **`/es` tree** with full parity and one source of truth for shared facts. Transcreate, don't machine-translate.

## Ticketing
AXS (Santa Barbara Bowl, event #1425277); currently reached via a `shorturl.at` redirect and an exposed raw AXS URL. → **IMPROVE**: branded, tracked deep links (UTMs); Spanish purchase path.

## System-wide issues to fix in migration
Generic slugs (`/new-page-1/2`, `/projects`, `/espanol` for an EN page); missing meta descriptions; `http` canonical; "© 2015/2026" and "27th/28th Anniversary" stale copy; image-baked text (sponsors, package, recommendations); EN/ES contradictions (board, years); GTM present but no evident conversion tracking.

## Migration summary
- **KEEP + IMPROVE:** Home, About, Board, Scholarships, Sponsors, Become a Sponsor, Contact, Gallery, Mariachi Recommendations.
- **RENAME:** `/espanol`→`/scholarships`, `/new-page-2`→`/gallery`, `/new-page-1`→`/community/mariachi-directory`, `/calendar`→`/events`.
- **SPLIT:** About→Mission/History/Board; Events→Upcoming/Past; Sponsorship→Our Sponsors/Become a Sponsor.
- **MERGE + REBUILD:** all Spanish pages → one `/es` tree.
- **REMOVE:** nothing outright (only ARCHIVE the Recommendations page if unmaintained).
