# Contributing to H3O Juice FL

Thank you for working on a real business project.

---

## Principles

1. **Honesty over hype** — Never present planned features as completed.
2. **Business first** — Code and design exist to support real juice sales and customers.
3. **Clarity for the next person** — Update docs when you change behavior or structure.
4. **Performance & accessibility matter** — Keep the site fast and usable.

---

## How to work

1. Read `docs/HANDOFF.md` and the relevant specialized doc first.
2. Prefer small, focused commits with clear messages.
3. Match the existing design tokens in `docs/DESIGN_SYSTEM.md`.
4. For images, follow `docs/IMAGE_GUIDELINES.md` strictly.
5. Test on mobile widths — most customers will be on phones.

---

## Code style (current stack)

- Single-page vanilla HTML + CSS + minimal JS.
- No build step required for the public site.
- Keep CSS variables and the `.glass` / `.glass-strong` utilities consistent.
- Prefer semantic HTML and existing class patterns over new inventiveness.

---

## Adding a new juice to the menu

1. Add a new `<article class="juice-card glass">` block in the menu section.
2. Use the same structure (media → title → description → price/tag).
3. When real photos exist, replace the emoji following IMAGE_GUIDELINES.

---

## Newsletter form

The form uses Formspree. Replace `YOUR_FORM_ID` in `index.html` with a real form ID from https://formspree.io (free tier is sufficient).

---

## Pull requests / handoff

If you are handing work to someone else:
- Update the status table in `docs/HANDOFF.md`.
- Note any open questions or blockers at the top of your PR or commit message.
- Leave the project in a runnable state.

---

## Questions

When in doubt, choose the simpler, more honest solution.