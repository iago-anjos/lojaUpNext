# Page Inspection — Narrow (320px–720px)

> **Method:** Chrome DevTools emulation with iPhone mobile user-agent  
> (`Mozilla/5.0 (iPhone; CPU iPhone OS 16_0 like Mac OS X) … Mobile/15E148 Safari/604.1`)  
> Screenshots saved to `audit/screenshots/narrow-{W}.png` (top) and `narrow-{W}-bottom.png` (bottom).  
> Note: VTEX IO uses UA-sniffing to serve mobile layout; a mobile UA was required for widths ≤ 620px to receive the mobile template.

---

## 320px
- **Overflow:** No (scrollWidth 320px, viewport 320px)
- **Page height:** ~8 284px
- **Layout template:** Mobile (hamburger header)
- **Issues:**
  1. **Benefícios block — aggressive text wrapping.** The four benefit items (MELHOR FRETE, DESCONTOS ESPECIAIS, ENTREGA EXPRESSA, PARCELE EM ATÉ 6X) render in a single narrow column. Text wraps to 2–3 lines per item, creating a very tall stacked block with poor visual hierarchy.
  2. **Category cards clipped.** The "Masculino" and "Feminino" category image cards are cut at the right edge — the image does not fully fit within the 320px column and appears cropped.
  3. **Footer contact icons misaligned.** In the ATENDIMENTO section, the phone/WhatsApp/email icons appear on a separate line above the corresponding text (e.g. icon on line 1, "(11) 3333-3333" on line 2). They should be inline.
  4. **Social icons vertical stack.** REDES SOCIAIS (Instagram, TikTok, Facebook, Blogger) are stacked vertically one per row, taking up excessive vertical space.
  5. **Newsletter text truncation.** The subtitle "Receba ofertas recomendadas e preços exclusivos" wraps to a second line, and at some render states the line was clipped.
  6. **Header:** "Minha Sacola" text label is visible next to the bag icon at the smallest width — at 320px this pushes the logo off-center.

---

## 420px
- **Overflow:** No (scrollWidth 420px, viewport 420px)
- **Page height:** ~8 678px
- **Layout template:** Mobile (hamburger header)
- **Issues:**
  1. **Footer contact icons misaligned.** Same as 320px — icons render on a separate line from the associated phone/WhatsApp/email text.
  2. **Social icons vertical stack.** Instagram, TikTok, Facebook, Blogger icons remain in a single vertical column. At 420px there is enough horizontal space to show them in a row.
  3. **Newsletter section:** Input field + CADASTRAR button render as a row — functional at this width. No overflow.
  4. **Benefícios block** text wrapping improves slightly over 320px but each item still occupies 2 lines.
  5. No critical overflow or hidden content found.

---

## 520px
- **Overflow:** No (scrollWidth 520px, viewport 520px)
- **Page height:** ~8 335px
- **Layout template:** Mobile (hamburger header)
- **Issues:**
  1. **Footer contact icons misaligned.** Same issue persists — icons float to their own line.
  2. **Social icons vertical stack.** Still stacked vertically; three icons could fit in a row at 520px.
  3. **Benefícios block** fully readable at this width with single-line labels; no wrapping issues.
  4. **Category section** images display at correct proportions.
  5. No critical overflow or hidden content found.

---

## 620px
- **Overflow:** No (scrollWidth 620px, viewport 620px — confirmed at page load; mid-session emulation reset to 768px for some evaluate_script calls but screenshot was taken at correct 620px width)
- **Page height:** ~6 679px (re-rendered at 768px for the scroll/bottom measurement — data approximate)
- **Layout template:** Mobile (hamburger header)
- **Issues:**
  1. **Footer contact icons misaligned.** Same icon/text alignment issue.
  2. **Social icons vertical stack.** Instagram, TikTok, Facebook, Blogger icons remain in a single vertical column despite ample width.
  3. **Newsletter section:** Input + button row fits well with good spacing. No issues.
  4. **Above product-images section** (near bottom): There is a large empty white space between the last product section and the newsletter block — likely a component with no content (empty shelf or placeholder).
  5. No overflow detected.

---

## 720px
- **Overflow:** No (scrollWidth 720px, viewport 720px)
- **Page height:** ~6 571px
- **Layout template:** **Desktop** (full horizontal nav, topbar visible — breakpoint crossed between 620px and 720px)
- **Issues:**
  1. **Desktop nav is cramped at 720px.** The horizontal category menu (Bolsas, Mochilas, Calçados, Esportivo, Eletrônicos, Itens) fits in one row but with very tight spacing. Some labels risk truncation on slightly narrower variants.
  2. **Topbar** (top bar with phone/social links) is visible and legible, though links are tightly packed.
  3. **Footer multi-column layout** (INSTITUCIONAL / REDES SOCIAIS / ATENDIMENTO / SELOS) renders in a 4-column row. The ATENDIMENTO column text wraps heavily — "Dúvidas sobre produtos e serviço de entrega?" wraps to 3 lines in a narrow column.
  4. **Social icons in footer** now render as a 2×2 grid (Instagram + TikTok on row 1, Facebook + Blogger on row 2) — better than the vertical stack at smaller widths but still not a single row.
  5. **Hero banner** renders in widescreen ratio at 720px with the desktop image — correct behavior.
  6. No overflow detected.

---

## Summary of Cross-Width Issues

| Issue | 320 | 420 | 520 | 620 | 720 |
|---|:---:|:---:|:---:|:---:|:---:|
| Footer contact icons misaligned (icon/text on separate lines) | X | X | X | X | — |
| Social icons in vertical stack instead of row | X | X | X | X | partial |
| Benefícios block text wraps aggressively | X | X | — | — | — |
| Category card images clipped | X | — | — | — | — |
| Large empty whitespace before newsletter | — | — | — | X | — |
| Desktop nav cramped at smallest desktop width | — | — | — | — | X |
| Footer ATENDIMENTO column text wraps to 3+ lines | — | — | — | — | X |

### Mobile breakpoint
The store switches from **mobile layout (hamburger)** to **desktop layout (horizontal nav)** somewhere between **620px and 720px**. At 720px the desktop layout is active. There is no intermediate tablet layout — this is an abrupt jump that may cause usability issues on ~650–719px devices (e.g. large phones in landscape).

### No horizontal overflow detected at any tested width.
