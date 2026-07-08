# LIVE-SITE-CONTENT-MAP.md
### Migration map from the current live site → redesigned institutional site
*Source re-audited: https://www.thesantabarbaramariachifestival.org/ (Squarespace). The redesign must carry this content forward — improved, not erased. Disposition = KEEP / IMPROVE / MERGE / RENAME / ARCHIVE / REMOVE.*

| Current page (URL) | What's there now | Disposition | New home |
|---|---|---|---|
| Home `/` | Wedding-photo hero, Spanish CTA to a shortlink, exposed AXS URL, "29 years" | **IMPROVE** (rebuild) | **Home** (institutional homepage) |
| About Us `/projects` | Mission statement; "From 1995 to today"; co-founders Salud Carbajal & Al Pizano; 29 yrs; César Chávez quote; real gallery photos | **KEEP + IMPROVE** | **About › Mission** + **About › History** |
| Board of Directors `/board` | Leadership list (all-volunteer) | **KEEP + MERGE** | **About › Board / Leadership** (single source of truth to end EN/ES contradiction) |
| Scholarships `/espanol` *(mislabeled slug)* | Scholarship mission, reception galleries, $ figure | **KEEP + IMPROVE + RENAME** → `/scholarships` | **Scholarships › Program** (+ new Impact, Recipient Stories) |
| Our Sponsors `/our-sponsors` | ~30 sponsor logos as screenshots | **KEEP + IMPROVE** (clean SVGs, tiers) | **Sponsorship › Our Sponsors** |
| Become a Sponsor `/sponsors` | Screenshot package, no form | **KEEP + IMPROVE** (real deck + inquiry form) | **Sponsorship › Become a Sponsor** |
| Upcoming Events `/calendar` | Mixed past+future events; no ticket link | **KEEP + RENAME + SPLIT** | **Events › Upcoming** and **Events › Past** |
| 2025 Festival Photos `/new-page-2` | ~70–90 photos (RG Photography) | **KEEP + RENAME** (real slug) | **Gallery / Stories** |
| Mariachi Recommendations `/new-page-1` | Stub / community resource | **ARCHIVE unless maintained** | **Community › Recommendations** (only if the org will keep it current) |
| Contact Us `/contact` | Address, email (transposed mailto bug), socials | **KEEP + IMPROVE** (fix email) | **Contact** |
| Spanish pages `/projects-1`,`/board-1`,`/espanol-2`,`/our-sponsors-copy`,`/become-a-sponsor-copy`,`/contact-1`,`/eventos` | Drifting, partial, stale ("27 años", outdated board, 2025-only events) | **MERGE + REBUILD** | **Single `/es` tree with full parity** (transcreated, one source of truth) |
| — (new) | — | **ADD** | **2026 Festival hub**: Overview · Artists · Tickets · Schedule · Visit · FAQ |
| — (new) | — | **ADD** | **Scholarships › Impact & Recipient Stories** |

**Nothing is removed for design convenience.** The only true removal candidate is the empty "Mariachi Recommendations" stub, and only if the org won't maintain it.

## Proposed architecture (institution + annual edition)
```
Home
2026 Festival ▸  Overview · Artists · Tickets · Schedule · Plan Your Visit · FAQ
About ▸          Mission · History · Board of Directors
Scholarships ▸   Program · Impact · Recipient Stories · (Apply, if applicable)
Events ▸         Upcoming · Past
Gallery / Stories
Sponsorship ▸    Our Sponsors · Become a Sponsor
Community ▸      Mariachi Recommendations (conditional)
Contact
Español (full parallel /es tree)
```
Primary nav shows a subset (Festival · Scholarships · Legacy/About · Sponsors · Español · **Tickets**); the rest lives in structured sub-menus and the footer. The homepage represents the institution and features the 2026 edition; it must still make sense in September.
