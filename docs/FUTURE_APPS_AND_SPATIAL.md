# Future Apps, Liquid Glass & Spatial — H3O Juice FL

This document is the roadmap and technical brief for anyone building native experiences or spatial features later.

---

## 1. Philosophy

Start with the real business. Add technology only when it creates clear customer or operational value.

Recommended order:
1. Excellent mobile web (current) + PWA
2. Real photos + newsletter
3. Optional native app only if order volume / loyalty justifies it
4. Spatial / glasses experiences when hardware is mainstream and content is ready

---

## 2. Progressive Web App (near-term)

- `manifest.json` is already in the repo.
- Add icons (`assets/icons/icon-192.png`, `icon-512.png`) when ready.
- Optional: simple service worker for offline shell later.

This gives “Add to Home Screen” behavior without an App Store review cycle.

---

## 3. Native iOS / macOS app (when justified)

### Liquid Glass (Apple material)

Liquid Glass is Apple’s dynamic material (iOS 26+ / corresponding OS versions). It combines glass optical properties with fluidity.

**Rules for H3O:**
- Prefer **standard SwiftUI / UIKit components** — they adopt Liquid Glass automatically.
- For custom views use `.glassEffect()`, `GlassEffectContainer`, and official glass button styles.
- Follow Apple’s official docs:
  - [Adopting Liquid Glass](https://developer.apple.com/documentation/technologyoverviews/adopting-liquid-glass)
  - [Applying Liquid Glass to custom views](https://developer.apple.com/documentation/swiftui/applying-liquid-glass-to-custom-views)
- Do **not** over-apply. Apple guidance: use it to focus content, not decorate everything.

### Suggested first native scope
- Menu + locations
- Simple order or pre-order flow
- Newsletter / push opt-in
- Loyalty stamp or simple rewards (later)

Use SwiftUI. Keep design tokens aligned with `docs/DESIGN_SYSTEM.md`.

---

## 4. Spatial & glasses (medium / long term)

| Platform | Status (mid-2026) | H3O opportunity |
|----------|-------------------|-----------------|
| Meta Ray-Ban / Meta Glasses | Shipping | Content + discovery |
| Apple Vision Pro | Shipping (niche) | High-fidelity product experience |
| Apple smart glasses | Expected late 2027 | Future |
| WebXR | Production-ready | Browser AR product viewer *now* |

### Practical near-term spatial move
Prepare clean **glTF / GLB** 3D models of the bottles. These work in:
- WebXR product viewers
- Vision Pro Safari
- Future glasses experiences
- Marketing renders

Do not wait for Apple Glass to start asset discipline.

---

## 5. Cross-platform notes

- Keep product data (name, price, ingredients, image path) in a simple structured format (JSON or Markdown) so web, app, and future tools can share it.
- Never hard-code copy in three places if it can live in one source of truth.

---

## 6. What not to build yet

- Complex backend / inventory system before sales volume demands it
- Full native app just for the sake of having an app
- Heavy AR for novelty

Build only what serves real customers and the real operation.