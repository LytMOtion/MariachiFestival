# NEW-IA.md
### Information architecture — permanent institution + annual edition
*The core structural correction: separate the permanent organization from the current campaign. The homepage belongs to the institution; the concert gets its own edition space.*

---

## The two layers

**Layer A — The permanent institution** (evergreen; makes sense every day of the year)
Home · The Music · Scholarships · Legacy · Stories · Artists (current + archive) · About · Partners · Español

**Layer B — The current edition** (annual campaign; swapped each year via data)
`/2026` festival hub · Tickets/Seats · Schedule · Visit · FAQ — all conversion, all replaceable.

Every year, Layer B is duplicated to `/2027` and re-pointed; Layer A barely changes. Past editions fold into **Legacy** (`/legacy/2026`, `/legacy/2025`…), which is how the archive grows without maintenance debt.

---

## Primary navigation (permanent)

`The Music · Scholarships · Legacy · Stories · 2026 Festival ▸ · [ES] · Tickets`

- **Tickets** is the only visually emphasized action; it deep-links to the current edition's ticket flow.
- **2026 Festival** is a labeled entry to Layer B (label updates by year via data).
- **[ES]** is the persistent, context-aware language toggle (lands on the equivalent page).
- Utility (About, Partners, Contact, Media, Give) lives in the footer and secondary menus, not the primary bar.

---

## Sitemap

```
/                         Home — the permanent front door (the institution)
/the-music                What mariachi is; the festival's relationship to the form
/scholarships             Mission, model, impact, recipients, how to give / apply
/legacy                   1996 → present; archive; past editions index
   /legacy/2025           Archived edition (photos, lineup, recap)  … etc.
/stories                  Editorial features: recipients, artists, families, community
   /stories/<slug>        Individual long-form story
/artists                  Current lineup + growing artist archive
   /artists/<slug>        Individual artist chapter
/about                    Org, mission, board/leadership (single source of truth), Fiesta history
/partners                 Sponsors & long-term partners (current + legacy), become a partner
/give                     Standalone giving (scholarship fund)
/media                    Press kit, facts, approved assets, contacts
/contact                  Correct email, address, roles

/2026                     CURRENT EDITION hub (Layer B)
   /2026/tickets          Seats, tiers, prices, buy (AXS)
   /2026/schedule         Running order, gates/show, day-of
   /2026/visit            Directions, parking, food, accessibility, family
   /2026/faq              Objection-busting
   (/2026/lineup redirects into /artists filtered to the 2026 edition)

/es/…                     Full parallel Spanish tree (all of the above)
/archive/…                (internal) rejected/reference prototypes — never linked publicly
```

---

## Page purposes (delta from v1's flat list)

| Page | Layer | Purpose | Primary action |
|---|---|---|---|
| Home | A | Emotional introduction to the *institution*; route to mission and to the current edition | Explore / Tickets |
| The Music | A | Establish mariachi as serious living art and the festival's stewardship of it | Read on |
| Scholarships | A | The reason the festival exists; move donors and applicants | Give / Apply |
| Legacy | A | 29-year continuum; house every past edition; archive-as-present | Explore archive |
| Stories | A | Human, editorial proof (recipients, artists, families) — replaces "quote cards" | Read a story |
| Artists | A/B | Current lineup as this year's chapter; grows into an archive | Tickets |
| About | A | Org truth, leadership (one source of truth to end EN/ES contradictions) | Contact / Give |
| Partners | A | Recognize + recruit sponsors, editorially (no logo soup) | Become a partner |
| **/2026 hub** | B | The concert campaign, concentrated | Get tickets |
| /2026/tickets | B | Honest seat selection + conversion | Buy on AXS |
| /2026/visit | B | De-risk logistics | Get tickets |

**What's deliberately *not* on the homepage:** seat-tier pricing grids, seat maps, FAQs, countdowns-as-hero, and "buy" as the first message. All of that is conversion machinery and belongs on `/2026`. The homepage may *reference* the current edition and carry a single, earned ticket CTA — but it is not an AXS page.

**Governance:** a single CMS "Edition" document holds all annual data (year, dates, venue, lineup refs, prices, ticket URL, on-sale state). The homepage and `/2026` both read from it, so next year is a data change, not a redesign — and Layer A never goes stale.
