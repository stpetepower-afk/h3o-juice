# Copilot instructions — H3O Juice FL

You are working on a **real mobile juice business** repo (Tampa Bay & Central Florida).
Phone for orders/location: **813-629-1078**.

## Always read first
1. `AGENTS.md`
2. `docs/HANDOFF.md`
3. `docs/DESIGN_SYSTEM.md` (when touching visuals)

## Stack
- Single-page vanilla HTML/CSS/JS — **no frameworks, no build step**
- GitHub Pages
- FormSubmit for the H3O Circle VIP form (`#circle`)
- `location.json` drives the daily drop panel — **never hard-code daily location in HTML**

## Hard rules
- Prefer small, honest changes
- **Never invent features** listed as missing in HANDOFF (no SMS pipeline, no native app, no margin tools, no fake photos)
- Keep Liquid Glass aesthetic (existing `.glass` / CSS variables)
- Mobile-first; test mental model at ~375px width
- After meaningful changes, update the status notes in `docs/HANDOFF.md`

## Form facts (do not invent fields)
Current Circle form fields: **name** (required), **email** (required), **phone** (optional).
There is no “preferred contact method” select unless explicitly added in the issue.

## Location updates
Edit **only** `location.json`. The page fetches it automatically.

## Style
- Use existing CSS custom properties in `index.html`
- Do not add new CSS files or UI libraries
- Do not add dependencies

Built for a real 18-month business. Honesty over hype.