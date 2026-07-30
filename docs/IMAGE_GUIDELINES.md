# Image Guidelines — H3O Juice FL

Real photography is the highest-leverage visual upgrade. These rules keep the site fast and premium.

---

## 1. Required shots (priority)

1. **Hero / OG cover** — 1200×630 (and 2400×1260 @2x)  
   Lifestyle or product cluster. Used for social sharing + Open Graph.
2. **Individual juice bottles** — square (1:1), minimum 1200×1200  
   Clean background or subtle surface. One per menu item.
3. **Detail / process** (optional) — press, fruit, hands, location.

---

## 2. Technical requirements

| Rule | Spec |
|------|------|
| Format | WebP primary, JPEG fallback |
| Max dimension | 1600px on longest side for product cards |
| Quality | 80–85 for WebP |
| Naming | `green-machine.webp`, `citrus-surge.webp`, etc. |
| Location | `assets/images/` |
| Loading | Always `loading="lazy"` + `decoding="async"` except hero/OG |
| Responsive | Use `srcset` with 1x / 2x when possible |

### Example markup (replace emoji)

```html
<div class="juice-media">
  <img
    src="assets/images/green-machine.webp"
    srcset="assets/images/green-machine.webp 1x, assets/images/green-machine@2x.webp 2x"
    alt="Green Machine cold-pressed juice bottle"
    width="600"
    height="600"
    loading="lazy"
    decoding="async"
  />
</div>
```

---

## 3. Optimization workflow (recommended)

1. Shoot in natural light, consistent style.
2. Edit (color grade to match brand: cool greens, clean whites).
3. Export master PNG/TIFF.
4. Generate WebP + JPEG with tools such as:
   - Squoosh.app
   - ImageOptim + WebP converter
   - `cwebp` CLI
5. Commit both 1x and 2x versions if file size stays reasonable.

Target: each product card image under ~80–120 KB.

---

## 4. Placeholder policy

Until real photos exist, keep the emoji inside `.juice-media`.  
Do **not** use low-quality stock photos. Empty premium is better than generic stock.

---

## 5. OG / social image

Place at: `assets/images/og-cover.jpg` (or `.webp` + update meta tags).  
1200×630, under 300 KB ideal.