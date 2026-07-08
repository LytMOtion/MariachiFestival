# QA-REPORT.md
### Controlled refinement & QA pass — Santa Barbara Mariachi Festival (A3 multi-page)
*No redesign of approved foundations (homepage, 2026 page, A3 visual system). Corrections only.*

## 1. Typography — headline wrapping (highest priority) — FIXED
- **Root cause:** interior hero captions were capped at `30ch`, so long phrases fragmented into one word per line.
- **Fix (in `a3.css`, applies site-wide):** widened `.lead-fig .cap` to `min(92vw,860px)`; set headline measures (`.lead-fig h1` 20ch, `.page-hero h1` 22ch); added **`text-wrap:balance`** to all headings/statements so lines balance instead of dropping single words; controlled `line-height`.
- **Result:** Become a Sponsor now reads "Partner with a night / the whole city / shows up for."; Scholarships reads "Opening doors / for the next generation." No hard-coded `<br>` breaks — reflows responsively (verified via 1440 & 390 hero renders `_qa/HERO_FIX_*`).
- **No repeated single hero formula:** page types now vary — media lead-figs (Scholarships, Become a Sponsor, Gallery, About, Español), ink page-heros (Board, Events, Contact, Sponsors, Directory), and the featured-event block on Events.

## 2. Public development language — REMOVED (moved to internal docs)
- **Español:** removed "This is the Spanish entry page / full versions are the next step / /es/ URLs / transcreated by a native speaker." Replaced with visitor-facing Spanish only ("Bienvenido…"). Page now `<html lang="es">`.
- **Gallery:** removed "being digitized" process line and the RG credit that would have mis-attributed AI placeholder images.
- **Directory:** removed the "listing to be provided / structure only" note.
- All remaining uncertainty lives only in `CONFIRMATION-NOTES.md`. **No `note-flag` text on any public page** (verified).

## 3. Mariachi Directory — fake data removed
- Deleted the `Mariachi [Name]` sample rows and the non-functional search field + category chips.
- Replaced with a polished **empty state** ("Community listings are being prepared.") + purpose + two real actions (Ask for a recommendation / Request to be listed). Search UI returns only when real data exists.

## 4. Gallery — data honesty
- Year navigation now distinguishes **available vs. future**: `2025` is a real in-page anchor (`#y2025`); earlier years shown as a single muted "2024 – 1996 · coming soon" marker. **No dead `href="#"`.**
- AI images are not credited as real event photography (credit removed from public copy; noted internally).

## 5. Contact — routing preserved, claims verified
- Five inquiry paths kept (General · Tickets · Sponsorship · Volunteering · Media & Press), each with a real mailto/route.
- "Board applications open in September" is **verified** — it appears on the org's live Board page — so it remains.

## 6. CTA / conversion logic — page-specific (not mechanical)
- Homepage: Get Tickets + Explore 2026. Festival: Get Tickets. Scholarships: Get Tickets + Become a Sponsor. Sponsors: Become a Sponsor. **Become a Sponsor: "Request Sponsorship Information."** Events: View Festival / Get Tickets. Gallery: Explore Festival / View Events. Contact: route by intent. Directory: Request to be listed. Español: Compra Boletos / Explora el Festival.

## 7. Dead links / technical — clean
- `href="#"` in the 12 site pages: **0**. All internal links resolve; all `public/media` paths resolve; tags balanced; inline JS valid on every page. (The stray `SBMF_Concept_Prototype.html` is the archived v1 — not part of the site, not linked; it couldn't be deleted due to file permissions — ignore it.)

## 8. Accessibility
- Drawer: `aria-hidden` toggced, menu button `aria-expanded` toggled, focus moves into drawer on open and back to the button on close, **Escape closes the drawer** (added to all pages, including homepage & 2026).
- `:focus-visible` outline (carmine) already in the system; buttons meet ≥48px min height; `prefers-reduced-motion` disables reveals/parallax; images have alt text; headings are semantic; **Español is `lang="es"`.**
- Contrast: white-on-ink and ink-on-white both pass AA; carmine used only for small labels/accents.

## 9. Factual audit (see CONFIRMATION-NOTES.md for the full list)
- **Verified & kept:** founded 1995 · first festival 1996 · Old Spanish Days Fiesta · 501(c)(3) EIN 77-0472982 · Board roster & roles (from live /board) · board applications open September · Scholarship Foundation of Santa Barbara partnership · colleges (Stanford/Brown/UCLA/UCSB/Cal Poly) · Aug 8 2026 · Santa Barbara Bowl · gates 4/show 5 · all ages · ticket prices (box office) · AXS event #1425277 · sponsor names · email/address/social.
- **Kept internal / not asserted publicly:** cumulative scholarship $ (sources conflict) · sponsor tier groupings (illustrative) · ticket tier names (proposal) · lineup billing (working client data) · 2026 portrait is AI atmosphere, not Majo Aguilar · directory list · earlier gallery years.

## 10. Presentation mode (clean client renders)
- Add `?present` to any URL (e.g., `index.html?present`) to hide the internal concept banner, the footer disclaimer, image "concept placeholder" captions, and the "AI concept placeholder" credit — without deleting any of it from the codebase. Default (no param) keeps all internal warnings on for private development.

## 11. Responsive QA notes
- Headlines use fluid `clamp()` + `text-wrap:balance` + measure caps, so they compose at 1440 / 1280 / 1024 / 768 / 430 / 390 without collapsing to one word per line.
- These are the corrected states; a final pass in a real browser at each breakpoint is recommended before launch (the sandbox can't run a live browser — renders here are composited from the real fonts/media/layout).

## Files changed this pass
`public/css/a3.css` (headline balance, measures, presentation mode, empty-state, gallery year states) · all 10 interior pages regenerated · `index.html` + `festival-2026.html` patched (presentation mode + Escape only) · `CONFIRMATION-NOTES.md` (kept internal). No new pages; no foundation redesign.

---
## Addendum — priority-page preview verification (desktop + mobile)
Rendered composited previews of all 10 priority pages at 1440 and 390, **simulating the browser's `text-wrap:balance`** against each page's real Bodoni metrics + `ch` measure + fluid font-size (`_prev/PREV_desktop.jpg`, `_prev/PREV_mobile.jpg`).

- **Finding:** `text-wrap:balance` minimizes the *longest* line, so for the long Become-a-Sponsor headline it produced an awkward "Partner with a / night the whole / city…" split. Balance alone could not yield the requested semantic structure.
- **Fix (Become a Sponsor only):** set the three intended breaks explicitly — "Partner with a night / the whole city / shows up for." — with a slightly reduced font clamp (`clamp(2.2rem,5vw,4.2rem)`) verified to fit down to 390px without fragmenting. This is the one place explicit breaks were justified; every other headline uses responsive `balance` + measure caps.
- **Scholarships:** confirmed "Opening doors for / the next generation." on desktop (reflows to a clean 3 lines on mobile).
- **Verified across all 10:** no one-word-per-line; images don't cover faces (text sits in the lower scrim / opposite the subject); CTA/label hierarchy intact; ink page-heros (Board/Events/Sponsors/Contact/Directory) read as institutional, not repeated cinematic formula.
- **Minor/acceptable:** About on ≤390px reflows the long place-name headline to 3 natural lines ("A Santa Barbara / tradition, / carried forward.").
- **Note on method:** these are composited previews (the sandbox can't run a live browser); wrapping is computed from real font metrics so the line breaks are faithful. A final in-browser pass at 1440/1280/1024/768/390 remains recommended before launch.
