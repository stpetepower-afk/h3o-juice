# H3O Juice FL — Agent Instructions

Real mobile juice business (Tampa Bay & Central Florida).  
Phone / text for orders & location: **813-629-1078**

## Stack
- Single-page vanilla HTML / CSS / JS (no build step)
- GitHub Pages
- FormSubmit powers the H3O Circle VIP form
- `location.json` drives the daily drop panel

## Key files
| File | Purpose |
|------|--------|
| `index.html` | The live page |
| `location.json` | Daily location — edit this, not the HTML |
| `docs/HANDOFF.md` | Master status + how everything works |
| `docs/DESIGN_SYSTEM.md` | Colors, glass materials, tokens |
| `docs/IMAGE_GUIDELINES.md` | How to add real product photos |
| `docs/CONTRIBUTING.md` | Working rules for humans & agents |

## Rules
- Prefer small, honest changes
- Never claim unbuilt features as done
- Keep the Liquid Glass aesthetic (see DESIGN_SYSTEM)
- Mobile-first
- After meaningful work, update the status table in `docs/HANDOFF.md`

## Do not
- Add frameworks unless explicitly asked
- Invent SMS, loyalty, or ops systems that do not exist
- Use heavy libraries or large stock images

## Daily location update
Edit only `location.json` (status, location_name, county, hours, maps_link).  
The page loads it automatically.

## H3O Circle form
FormSubmit → currently `stpetepower@gmail.com`.  
Collects name, email (required), phone (optional). No automated SMS yet.

---
Built for a real 18-month juice business. All hands welcome. Mustard seed faith.