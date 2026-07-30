# H3O™ Copilot Agent System Instructions

## Primary Context & Ground Rules
Before making any changes or opening a PR, always read and adhere strictly to:
1. `AGENTS.md`
2. `docs/HANDOFF.md`
3. `docs/IMAGE_GUIDELINES.md`
4. `docs/DESIGN_SYSTEM.md` (when touching visuals)

## Key Operational & Brand Truths
- Brand Philosophy: "Born from a simple idea. Proven one bottle at a time."
- Sourcing: 100% Hand-pressed, raw fruit (**NEVER** refer to juices as "cold-pressed" or HPP).
- Products:
  1. H3O™ Seeded Watermelon Juice
  2. H3O™ Mango Pineapple Orange Juice
- Ordering & Contact: Phone/SMS line is **813-629-1078**.
- Regional Reach: 6-County coverage across Tampa Bay & Central Florida (Pinellas, Hillsborough, Pasco, Polk, Manatee, Orange/Orlando).
- Daily Drop Updates: Controlled exclusively via `location.json`. Do not hardcode static daily locations in HTML.

## Form facts (do not invent fields)
H3O Circle form fields: **name** (required), **email** (required), **phone** (optional).
FormSubmit backend — keep submission working. No automated SMS pipeline exists yet.

## Execution Constraints
- **No Unbuilt Features:** Do NOT invent unbuilt apps, fake menus, QR code passes, SMS systems, or external dependencies.
- **Zero Bloat:** Maintain pure, high-craft HTML/CSS/JS with zero third-party framework overhead unless explicitly instructed.
- **Styling:** Preserve the dark "Liquid Glass" theme, responsive CSS grid, and mobile-first glassmorphic layouts. Use existing CSS variables in `index.html`.
- **Images:** Use native `<img>` or `<picture>` tags with `loading="lazy"` and `decoding="async"`. No stock photos.
- After meaningful changes, update status notes in `docs/HANDOFF.md`.

Built for a real 18-month juice business. Honesty over hype.