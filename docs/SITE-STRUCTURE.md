# SITE-STRUCTURE.md
### Multi-page A3 website — structure, navigation, and confirmation notes
*Real multi-page site (not one long page) on the approved A3 visual system. Shared `public/css/a3.css` + self-hosted fonts. Every page has identical nav + footer linking to real pages.*

## File list (12 pages + system)
| File | Purpose | Source (migrates from) |
|---|---|---|
| `index.html` | Homepage — hero, 2026 preview, **routing** to interior pages, final CTA (not every detail) | `/` |
| `festival-2026.html` | Current festival — lineup, **tickets** (6 tiers + AXS), schedule, plan your visit, FAQ | `/calendar` + homepage |
| `about.html` | Mission, history, purpose, founding, community role | `/projects` |
| `board.html` | **Board of Directors** — full roster + roles, text-led leadership index, volunteer path | `/board` |
| `scholarships.html` | Program, who it serves, how to apply, Scholarship Foundation | `/espanol` (mislabeled) |
| `sponsors.html` | Sponsor recognition | `/our-sponsors` |
| `become-a-sponsor.html` | Why partner, request the package, inquiry CTA | `/sponsors` |
| `events.html` | Upcoming programming with hierarchy | `/calendar` |
| `gallery.html` | Festival photography + archive (by year) | `/new-page-2` |
| `mariachi-recommendations.html` | Community mariachi directory | `/new-page-1` |
| `contact.html` | Email, address, social, sponsorship & volunteer paths | `/contact` |
| `espanol.html` | Spanish landing + routing; full bilingual plan | `/…-1`, `/eventos`, etc. |
| `public/css/a3.css` | Shared design system (tokens, components, interior pages) | — |
| `public/fonts/*` | Self-hosted Bodoni Moda + Hanken Grotesk | — |

## Navigation (identical on every page)
- **Primary bar:** wordmark (→ index) · Festival · Scholarships · Board · Sponsors · **Español** · **Tickets** (white button → festival-2026#tickets).
- **Full menu (hamburger drawer):** Home · The 2026 Festival · About · Board of Directors · Scholarships · Events · Gallery · Sponsors · Become a Sponsor · Mariachi Directory · Contact · Español · **Get Tickets**.
- Language toggle swaps `data-en`/`data-es` site-wide; `espanol.html` is the Spanish front door.

## Footer (identical on every page)
Four columns linking to **real pages** — Festival (2026 Festival, Tickets, Events, Gallery) · Organization (About, Board of Directors, Scholarships, Mariachi Directory) · Connect (Our Sponsors, Become a Sponsor, Contact, email) · brand + Facebook/Instagram + address + EIN + the internal-concept disclaimer.

## Interior-page design system (added to a3.css)
`.page-hero` (ink or media-backed page header with breadcrumb + label + Bodoni title + lede) · `.prose` / `.two-col` (editorial body) · `.leaders` (text-led board index, officers + members with roles) · `.tiers` (seat/ticket list) · `.sched` (schedule) · `.faq` · `.info-grid` (visit/contact) · `.gal-grid` (archive) · `.dir` (directory) · `.routes` (homepage preview cards) · `.note-flag` (internal confirmation flags). Buttons follow the approved rule: **white on dark, ink on light; carmine reserved for labels.**

## Content confirmation notes (flagged in-page with `.note-flag`)
- **Board:** roster migrated verbatim from the live `/board` page (Miguel Martinez–President, Perla Navarro Lewis–VP, Erika Aldaz–Treasurer, Liz Ruiz–Secretary; members Miguel Avila, Joanna Contreras, Richard Garnica, Tere Jurado, Casie Killgore, Marco Menchaca, Carlos Pacheco). Real headshots exist (Richard Garnica / RG Photography) — a **text-led index** is used until those photos are licensed; volunteer/board form link is the real `forms.gle` URL.
- **Scholarships:** no cumulative dollar figure published (public sources conflict $650K+ vs $1M+ — reconcile). No recipient stories invented (real ones need written consent). Colleges (Stanford/Brown/UCLA) and the Scholarship Foundation partner are verified.
- **Tickets:** prices verified from the Santa Barbara Bowl public listing (box office); tier **names** are a concept proposal; AXS may add fees. Buy links point to AXS event #1425277.
- **Sponsors:** names are those publicly listed by the org; groupings are **illustrative, not verified tiers**; clean vector logos + confirmed tiers should replace before publication.
- **Events:** Winter Show / Vocal Competition / Aug 7 reception reflect the org's public calendar; details to confirm.
- **Mariachi Directory:** the live page invites groups to be listed by email; the actual list is **not reproduced** (would require migrating real names/contacts from the org).
- **Lineup:** Majo Aguilar · Joss Favela · Mariachi Los Camperos is working client data; the 2026 portrait is AI **atmosphere**, explicitly **not** Majo Aguilar (licensed media TBD).
- **Español:** a real front door + working toggle now; full per-page transcreation (parallel `/es/` URLs, native-speaker review) is the documented next step — not machine translation.

## Not done yet (next phase)
Full `/es/` page tree; real photography/logos/headshots; live analytics + AXS UTM deep links; CMS for the annual edition. Nothing here is published; the live site is untouched.
