# Santa Barbara Mariachi Festival — Website Concept (A3)

A complete, static, bilingual **concept redesign** of the Santa Barbara Mariachi Festival website — a 12‑page institutional site built on a refined editorial design system ("A3": deep ink · luminous mineral white · a single carmine accent · Bodoni Moda + Hanken Grotesk, self‑hosted).

> ⚠️ **Internal concept — not official.** This is an unsolicited design study. It is **not** authorized by, affiliated with, or endorsed by the Santa Barbara Mariachi Festival, Inc. **All imagery is temporary AI‑generated placeholder media** and must be replaced with real licensed photography before any public use. The 2026 portrait is **not** Majo Aguilar. See `docs/CONFIRMATION-NOTES.md` for every item that must be verified with the organization before launch.

## Quick start
It's plain static HTML/CSS — no build step.

```bash
# from the repo root
python3 -m http.server 8000
# then open http://localhost:8000
```

Or just open `index.html` in a browser. Keep the `public/` folder next to the HTML.

**Presentation mode:** add `?present` to any URL (e.g. `index.html?present`) to hide the internal concept banner, footer disclaimer, and placeholder captions for clean client‑facing views.

## Structure
```
index.html                     Home (routes to the rest)
festival-2026.html             Current edition — lineup, tickets, schedule, visit, FAQ
about.html                     Mission, history, purpose
board.html                     Board of Directors (real roster)
scholarships.html              Program, how it works, impact
sponsors.html                  Sponsor recognition
become-a-sponsor.html          Partnership / conversion
events.html                    Upcoming programming
gallery.html                   Photography & archive
mariachi-recommendations.html  Community directory
contact.html                   Inquiry routing
espanol.html                   Spanish landing (lang="es")
public/css/a3.css              Design system
public/fonts/                  Self‑hosted Bodoni Moda + Hanken Grotesk (OFL)
public/media/                  AI placeholder imagery/video (replace before launch)
docs/                          Research, strategy, QA, and confirmation notes
```

## GitHub Pages
Push to a repo and enable **Settings → Pages → Deploy from branch → root**. `index.html` is at the repo root, so it serves as‑is.

## Tech
Static HTML + one CSS file. Self‑hosted variable/static fonts (SIL Open Font License): **Bodoni Moda** (display) and **Hanken Grotesk** (text). Bilingual EN/ES via `data-en`/`data-es` toggling. Accessible drawer (aria + Escape), `prefers-reduced-motion` support, `text-wrap:balance` headlines.

## Before publishing — must confirm with the organization
- Final **2026 lineup** and billing order (currently working client data).
- Replace **all AI imagery** with licensed photography (esp. the 2026 artist media and Board headshots).
- **Scholarship figures** (public sources conflict; none published here on purpose).
- **Sponsor roster/tiers** (groupings here are illustrative), clean vector logos.
- **Mariachi directory** real listings.
- Ticket **tier names** (concept proposal) and any AXS fees; prices are from the venue's public box‑office listing.

Full checklist: `docs/CONFIRMATION-NOTES.md`. Design/QA rationale: `docs/QA-REPORT.md`, `docs/SITE-STRUCTURE.md`.
