# Design System — H3O Juice FL

## Brand essence
Honest. Premium. Local. Zero hype. Real juice that earns its place.

---

## Color tokens

| Token | Value | Usage |
|-------|-------|-------|
| `--bg` | `#0c100e` | Page background |
| `--bg-elevated` | `#121816` | Elevated surfaces |
| `--surface` / glass | `rgba(26,33,28,0.55)` + blur | Cards, panels |
| `--text` | `#f4f1ea` | Primary text |
| `--text-muted` | `#a8b0a4` | Secondary text |
| `--accent` | `#7cb342` | Primary actions, highlights |
| `--accent-soft` | `#9ccc65` | Hover / softer accent |
| `--gold` | `#e8c47c` | Prices, stats, emphasis |
| `--glass-border` | `rgba(255,255,255,0.12)` | Glass edges |
| `--glass-highlight` | `rgba(255,255,255,0.18)` | Inset top highlight |

---

## Typography

- **Display / Headings:** Playfair Display (serif), weights 500–700  
- **Body / UI:** DM Sans, weights 400–700  
- Fluid type scale using `clamp()` for headings.

---

## Materials (Liquid Glass–inspired for web)

### `.glass`
```css
background: rgba(255,255,255,0.06);
backdrop-filter: blur(24px) saturate(1.4);
border: 1px solid rgba(255,255,255,0.12);
box-shadow: 0 4px 24px rgba(0,0,0,0.25), inset 0 1px 0 rgba(255,255,255,0.18);
```

### `.glass-strong`
Stronger blur + slightly higher opacity. Use for primary panels (newsletter, key CTAs).

**Rules**
- Prefer glass on interactive or elevated surfaces only.
- Do not apply glass to every element (Apple guidance: avoid overuse).
- Always provide a solid fallback background for browsers without `backdrop-filter`.

---

## Spacing & radius

- Radius: `20px` (cards), `12px` (inner media), `999px` (pills/buttons)
- Section padding: `5rem 1.5rem`
- Consistent gap scale: 0.75 / 1 / 1.25 / 1.75 / 2.5 rem

---

## Motion

- Prefer 0.2–0.25s ease transitions.
- Respect `prefers-reduced-motion`.
- Subtle hover lift (`translateY(-2px to -4px)`) + glow on primary actions.

---

## Accessibility

- Maintain WCAG AA contrast on text.
- Focus rings visible (accent glow on inputs).
- Semantic HTML + ARIA where needed.
- Skip link present.

---

## Future native (Apple Liquid Glass)

When building with SwiftUI (iOS 26+):
- Prefer standard components — they adopt Liquid Glass automatically.
- For custom views use `.glassEffect()` and `GlassEffectContainer` sparingly.
- Follow Apple’s “Adopting Liquid Glass” documentation exactly.
- Do not invent custom materials that fight the system.

See `docs/FUTURE_APPS_AND_SPATIAL.md` for more.