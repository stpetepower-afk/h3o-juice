# H3O Juice FL — Master Handoff

**Last updated:** 2026-07-30  
**Repo:** https://github.com/stpetepower-afk/h3o-juice  
**Live (after Pages enabled):** https://stpetepower-afk.github.io/h3o-juice/

This document is the single source of truth for any developer, designer, or creator joining the project — anywhere in the world.

---

## 1. What this project is

H3O Juice FL is a **real operating juice business** (18+ months, 6 days/week, Tampa Bay & Central Florida).  
Mobile operation: hand-pressed juice (Seeded Watermelon + Mango·Pineapple·Orange), sold from coolers.  
Phone for orders/location: **813-629-1078**.

**Core philosophy:** Real product first. Software supports the business; it does not pretend to be the business.

---

## 2. Current honest status

| Area | Status | Notes |
|------|--------|-------|
| Website (single page) | ✅ Built | Liquid Glass–inspired design |
| Deployed / live | ⏳ Pending | Enable GitHub Pages (see README) |
| Real product photos | ❌ Missing | Emoji placeholders only |
| H3O Circle VIP form | ✅ Live | FormSubmit → stpetepower@gmail.com |
| Daily location system | ✅ Live | Edit `location.json` only |
| Social handles claimed | ❌ Pending | Target: @h3ojuicefl |
| Native app | ❌ Not started | See FUTURE_APPS_AND_SPATIAL.md |
| Automated SMS pipeline | ❌ Not started | Form collects optional phone; no auto-SMS yet |
| Ops / margin tools | ❌ Not started | Future |

---

## 3. Repository structure

```
h3o-juice/
├─ index.html              # Live page (Liquid Glass aesthetic)
├─ location.json           # Daily drop status — edit this, not the HTML
├─ manifest.json           # PWA manifest
├─ README.md               # Quick start + Pages instructions
├─ docs/
│   ├─ HANDOFF.md         # This file
│   ├─ DESIGN_SYSTEM.md   # Colors, type, materials, spacing
│   ├─ IMAGE_GUIDELINES.md# How to add optimized photos
│   ├─ INSTAGRAM_PROFILE.md # Complete social system
│   ├─ FUTURE_APPS_AND_SPATIAL.md
│   └─ CONTRIBUTING.md
└─ assets/                # (create when photos arrive)
    ├─ images/
    └─ icons/
```

---

## 4. Daily operations (location)

**To update today’s stop** (takes ~20 seconds):

1. Open `location.json`
2. Edit these fields:
   - `status` — e.g. `"LIVE NOW · FRESH BATCH READY"`
   - `location_name` — e.g. `"Downtown Fresh Market Setup"`
   - `county` — e.g. `"Pinellas County"`
   - `hours` — e.g. `"8:00 AM – 2:00 PM Today"`
   - `maps_link` — Apple/Google Maps URL
3. Commit / save

The page reads this file automatically. No need to touch `index.html`.

---

## 5. H3O Circle™ VIP form

- Collects: first name, email (required), phone (optional)
- Backend: **FormSubmit** → currently `stpetepower@gmail.com`
- First submission triggers a one-time confirmation email from FormSubmit — click the link to activate
- To change destination email: edit the `action` attribute on the form in `index.html`  
  `https://formsubmit.co/YOUR_EMAIL@example.com`

There is **no automated SMS system** yet. Phone numbers land in the email so you can text people manually or later connect a real SMS tool.

---

## 6. Immediate next actions (priority order)

1. **Enable GitHub Pages** (30 seconds) — see README.md  
2. **Claim social handles** (`@h3ojuicefl`)  
3. **Take real product photos** → `docs/IMAGE_GUIDELINES.md`  
4. **Confirm FormSubmit** by submitting a test signup and clicking the activation email  
5. **Update `location.json`** with a real today’s stop  
6. **Add OG image** (`assets/images/og-cover.jpg` — 1200×630)  

---

## 7. Design direction

- **Web:** Liquid Glass–inspired (translucent surfaces, blur, depth, fluid interaction).  
- **Native (future):** Full Apple Liquid Glass material via SwiftUI.  
- **Brand voice:** Honest, calm, premium, zero hype.  
- **Visual:** Dark base, soft green accent, gold highlights, glass materials.

Full tokens: `docs/DESIGN_SYSTEM.md`.

---

## 8. Contact & ownership

- GitHub owner: `stpetepower-afk`  
- Business phone: 813-629-1078  
- Business: H3O Juice FL, Tampa Bay & Central Florida  

When you finish meaningful work, update this status table and the relevant specialized doc.

---

**Thank you for treating this like a real business, not a demo.**