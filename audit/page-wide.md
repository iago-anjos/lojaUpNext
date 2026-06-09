# Page Inspection — Wide (768px–1440px)

**Store URL:** https://iagoupnext--upnext.myvtex.com/
**Audit date:** 2026-05-27
**Method:** Chrome DevTools emulation, desktop UA (`Windows NT 10.0; Chrome/124`), desktop DPR=1, no touch/mobile flags.
**Note on scrollWidth delta:** At every width, `scrollWidth` reads ~15px less than `innerWidth`. This is the native scrollbar gutter, not a content overflow — no horizontal scrollbar was triggered at any breakpoint.

---

## 768px

- **Viewport confirmed:** 768px (innerWidth=768, scrollWidth=753)
- **Horizontal overflow:** No
- **Issues:**
  - VTEX initially served mobile layout (iPhone UA 720px) when `emulate` was called without explicit desktop UA; required explicit UA override + reload to get desktop rendering. This means the 768px breakpoint is fragile — if the browser UA changes, VTEX may serve the mobile template.
  - Product shelf renders **2 cards per row** at this width (vs 3 at wider viewports). This is technically a VTEX responsive-layout breakpoint boundary and may be intentional, but the shelf feels sparse with 2 wide cards.
  - Info bar: 4 columns visible but text labels are tight/abbreviated — "para todo o Brasil", "para compras em volume" text is clipped in smaller fonts.
- **Header:** OK — topbar (phone + "Ver Ofertas"), logo, search bar, user/cart icons, category nav (6 items) all visible and fitting.
- **Hero banner:** OK — full-width, "OUTLET 50% OFF / CONFIRA" text centered and readable.
- **Info bar:** 4 columns present (MELHOR FRETE+, DESCONTOS ESPECIAIS, ENTREGA EXPRESSA, PARCELE EM ATÉ 6X) — slightly compressed but not broken.
- **Category cards / seasonal banners:** 2-column grid (MODA OUTONO, MODA INVERNO visible) — correct layout.
- **Product shelf:** 2 cards per row — Feminino and Acessórios shelves both render 2-up.
- **About Us:** Text fits within container, no overflow, dark maroon background with white text readable.
- **Newsletter:** Row layout — icon/text on left, email input + CADASTRAR button on right. OK.
- **Footer:** 4 columns (INSTITUCIONAL, REDES SOCIAIS, ATENDIMENTO, SELOS) — all fitting, no wrapping into single column.

---

## 868px

- **Viewport confirmed:** 868px (innerWidth=868, scrollWidth=853)
- **Horizontal overflow:** No
- **Issues:**
  - None critical. Product shelf still 2 cards per row — the 2→3 column transition has not yet triggered.
  - Info bar: 4 columns, text slightly less compressed than at 768px.
- **Header:** OK — all topbar/logo/search/nav elements fitting cleanly.
- **Hero banner:** OK — proportions good, full-width.
- **Info bar:** 4 columns, readable.
- **Product shelf:** 2 cards per row (same as 768px — breakpoint transition to 3-up has not triggered yet at 868px).
- **About Us:** OK.
- **Newsletter:** Row layout, OK.
- **Footer:** 4 columns, fitting well.

---

## 968px

- **Viewport confirmed:** 968px (innerWidth=968, scrollWidth=953)
- **Horizontal overflow:** No
- **Issues:**
  - None. Layout is stable.
  - Product shelf transitions to **3 cards per row** at approximately this breakpoint.
- **Header:** OK — topbar, logo, search bar with more room, category nav all fitting.
- **Hero banner:** OK — full-width, proportional.
- **Info bar:** 4 columns, comfortable spacing.
- **Product shelf:** 3 cards per row — correct desktop layout.
- **About Us:** OK.
- **Newsletter:** Row layout, OK.
- **Footer:** 4 columns, OK.

---

## 1068px

- **Viewport confirmed:** 1068px (innerWidth=1068, scrollWidth=1053)
- **Horizontal overflow:** No
- **Issues:**
  - None. All sections stable and well-proportioned.
- **Header:** OK — logo, search bar, icons, nav all comfortable.
- **Hero banner:** OK — full-width.
- **Info bar:** 4 columns, well spaced.
- **Product shelf:** 3 cards per row.
- **About Us:** Text content visible above newsletter, no overflow.
- **Newsletter:** Row layout (icon+text left, input+button right).
- **Footer:** 4 columns (INSTITUCIONAL, REDES SOCIAIS, ATENDIMENTO, SELOS) — all fitting with good spacing.

---

## 1168px

- **Viewport confirmed:** 1168px (innerWidth=1168, scrollWidth=1153)
- **Horizontal overflow:** No
- **Issues:**
  - None. Solid desktop layout across all sections.
- **Header:** OK — all elements have room, search bar comfortable width.
- **Hero banner:** OK.
- **Info bar:** 4 columns, well padded.
- **Product shelf:** 3 cards per row.
- **About Us:** OK.
- **Newsletter:** Row layout, OK.
- **Footer:** 4 columns, OK.

---

## 1268px

- **Viewport confirmed:** 1268px (innerWidth=1268, scrollWidth=1253)
- **Horizontal overflow:** No
- **Issues:**
  - None. Page is well-behaved.
- **Header:** OK.
- **Hero banner:** OK — banner fills width, text centered.
- **Info bar:** 4 columns, comfortable.
- **Product shelf:** 3 cards per row.
- **About Us:** OK — text paragraph fits, no overflow.
- **Newsletter:** Row layout, OK.
- **Footer:** 4 columns, OK.

---

## 1368px

- **Viewport confirmed:** 1368px (innerWidth=1368, scrollWidth=1353)
- **Horizontal overflow:** No
- **Issues:**
  - None critical. The layout appears to have reached its max-width content container — sections do not stretch beyond the container max-width.
- **Header:** OK — topbar ("Atendimento (41) 9999-9999" + "Ver Ofertas"), logo, search, user/cart, category nav (Beleza, Mindset, Calçados, Esportivo, Eletrônicos, Jeans) all visible.
- **Hero banner:** OK — full-width background, centered text.
- **Info bar:** 4 columns with comfortable spacing.
- **Product shelf:** 3 cards per row.
- **About Us:** OK.
- **Newsletter:** Row layout, button clearly visible.
- **Footer:** 4 columns, fitting well with good white space.

---

## 1440px

- **Viewport confirmed:** 1440px (innerWidth=1440, scrollWidth=1425)
- **Horizontal overflow:** No
- **Issues:**
  - None. This is the primary design width and everything is at its best.
- **Header:** OK — all elements present, well spaced. Category nav shows all 6 items with comfortable gaps.
- **Hero banner:** OK — full-width, proportional height, text overlay centered.
- **Info bar:** 4 columns (MELHOR FRETE+, DESCONTOS ESPECIAIS, ENTREGA EXPRESSA, PARCELE EM ATÉ 6X) — well spaced, all labels readable.
- **Category cards / seasonal banners:** 2-column seasonal banners (MODA OUTONO / MODA INVERNO) — correct grid.
- **Product shelf:** 3 cards per row (Feminino, Infantil, Acessórios shelves all confirmed 3-up).
- **About Us:** Dark maroon section with upnext logo and text — no overflow, text fits within container, image visible to the right.
- **Newsletter:** Row layout — icon, "Se conecte com a gente!" heading, subtitle on left; email input + CADASTRAR button on right.
- **Footer:** 4 columns (INSTITUCIONAL, REDES SOCIAIS, ATENDIMENTO, SELOS) with comfortable spacing and full copyright bar below.

---

## Summary of Issues by Severity

### HIGH
- None found.

### MEDIUM
- **768px — VTEX mobile/desktop template boundary:** At exactly 768px, VTEX may serve the mobile template depending on the browser UA. The emulated desktop UA rendered the desktop template correctly, but a real tablet browser with a mobile UA would receive the mobile layout. The breakpoint logic is based on UA detection in addition to viewport width. If tablet users should see the desktop layout, this needs attention in `responsive-layout` block configuration.

### LOW
- **768–868px — Product shelf 2 cards per row:** The product shelf renders 2 items per row at 768–868px. At 968px it transitions to 3-up. The 2-column shelf at tablet widths looks sparse with large cards. Consider whether the `responsive-layout.tablet` breakpoint should show 3 columns or if 2 is intentional.
- **768px — Info bar text compression:** The 4-column info bar is slightly compressed at 768px with text slightly tight, though not clipped or overflowing.
- **All widths — scrollWidth is ~15px less than innerWidth:** This delta is consistent across all widths and equals the browser scrollbar gutter width. No action needed — this is expected browser behavior.

### INFORMATIONAL
- Page height ranges from ~5,970px (1068px) to ~6,740px (768px) — the taller page at narrower widths is due to the 2-column product shelf stacking more rows.
- The topbar "Ver Ofertas" pill button is present and correctly styled at all widths.
- Footer social icons (Instagram, TikTok, Facebook, Blogger) render correctly at all widths.
- Payment icons (Visa, Mastercard, Boleto) in the footer bottom bar are present at all widths.
