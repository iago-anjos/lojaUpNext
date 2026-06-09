# UpNext VTEX IO — Figma Mobile Audit
**Figma File:** `ZLRnvrtFM3l4srJgsww44W`  
**Mobile Homepage Frame:** `1:265` — `upnext-HOME-mobile`  
**Frame Dimensions:** 360 × 5277 px  
**Date:** 2026-05-27

---

## 1. Mobile Header (Topbar + Header Bar)

### 1a. Info Bar (Frete Grátis Strip)
Node: `2741:8` — `topo` (desktop version shown; mobile has equivalent strip)

| Property | Value |
|----------|-------|
| Background | `#8B1A4A` (dark magenta/maroon) |
| Height | 29px |
| Width | 360px (full width) |
| Text | "Faltam R$149,99 para ganhar FRETE GRÁTIS" |
| Text color | `#FFFFFF` |
| Font size | ~12px |
| Font weight | Regular |
| Icon | Truck icon (white), left of text |
| Layout | Row, centered horizontally |

### 1b. Header Bar
Node: `2808:233` — `topo` (360 × 63px)

| Property | Value |
|----------|-------|
| Background | `#8B1A4A` (dark magenta/maroon — approx `#8C1A47`) |
| Height | 63px |
| Width | 360px |
| Logo | UpNext white logo, left-aligned (163 × 52px approx) |
| Logo position | Left, vertically centered |
| Search icon | White magnifying glass, right side |
| User/Login icon | White person icon, right side |
| Cart icon | White bag icon with badge "01", right side |
| Hamburger menu | White 3-line icon, far right |
| Icon spacing | ~8px gap between icons |
| Icons area | Right side, horizontally aligned row |
| Border | None |
| Box-shadow | None visible |

---

## 2. Hero Banner (Banner Principal)
Node: `1:266` — `banner principal` (360 × 404px)

| Property | Value |
|----------|-------|
| Width | 360px |
| Height | 404px (visible area) |
| Background | `#8C1A47` (dark magenta) — left half |
| Background right | White/light (product image area) |
| Layout | Split: text left, product image right |
| Headline text | "Viva as coisas boas da Vida" |
| Headline font | Script/cursive font (decorative) |
| Headline size | ~32px |
| Headline color | `#FFFFFF` |
| Banner image | Product photo (plant/vase) on grey patterned background |
| Navigation arrows | Left/right chevron arrows, white on semi-transparent dark circle |
| Arrow size | ~30px diameter |
| Dot indicators | 3 dots at bottom, active dot is magenta/dark, inactive is lighter |
| Dot size | ~8px diameter |
| Dot gap | ~6px |
| Padding | ~18px left padding on text side |
| Slide transition | Horizontal carousel |

---

## 3. Benefits / Info Bar
Node: within `1:265` (visible in full page screenshot at approx y=420–500)

| Property | Value |
|----------|-------|
| Width | 360px |
| Height | ~80px |
| Background | `#F5F5F5` (light grey) |
| Layout | Row, 3 or 4 benefit items centered |
| Items | Frete grátis, Parcelamento, Devolução, Segurança |
| Icon size | ~24px |
| Icon color | `#8C1A47` (magenta) |
| Text size | ~10–11px |
| Text color | `#333333` |
| Text weight | Regular/Medium |
| Gap between items | Equal spacing |
| Border | None |

---

## 4. RESTOFF Countdown / Deals Timer
Node: within `1:265` (visible in full page screenshot, approx y=500)

| Property | Value |
|----------|-------|
| Width | 360px |
| Height | ~60px |
| Background | `#F5F5F5` or white |
| Label | "RESTOFF" badge (yellow/green badge) |
| Timer | Format: "08h : 18min : 36s" |
| Timer background | Dark/black boxes for each unit |
| Timer text | White, bold, monospace-style |
| Timer text size | ~16px |
| Label text | Bold, uppercase |
| Layout | Row, left-aligned label + timer |
| Padding horizontal | ~10px |

---

## 5. Product Shelf — "SUPER OFERTAS"
Node: `2727:55` (shelf component, 341 × 462px)

| Property | Value |
|----------|-------|
| Width | 360px (full) |
| Section height | ~520px |
| Background | `#FFFFFF` |
| Section title | "SUPER OFERTAS" |
| Title font | Bold, sans-serif |
| Title size | ~16px |
| Title color | `#222222` |
| Title decoration | Magenta `#8C1A47` left bar/accent |
| Items per row | 2 |
| Card width | ~160px |
| Card height | ~220px |
| Card background | `#FFFFFF` |
| Card border | None / very subtle |
| Card border-radius | ~4px |
| Product image size | ~160 × 160px |
| Product name | ~12px, regular, dark grey |
| Price (original) | Strikethrough, ~11px, grey |
| Price (sale) | Bold, ~14px, `#222222` |
| Installments text | ~10px, grey |
| CTA button | Green `#27AE60`, "COMPRAR", full width, ~30px height |
| CTA font | Bold, ~11px, white |
| CTA border-radius | ~4px |
| Badge "Outlet" | Small label, top-left of image, yellow or orange bg |
| Badge "Lançamento" | Small label, yellow bg, `#F2C94C` |
| Navigation arrows | Left/right chevrons on sides of carousel |
| Dot indicators | Magenta active, grey inactive |
| Gap between cards | ~8–10px |
| Padding horizontal | ~10px |

---

## 6. Category Cards Section
Node: within `1:265` (visible at ~y=1400–1600 in mobile page)

| Property | Value |
|----------|-------|
| Width | 360px |
| Section height | ~200px |
| Background | `#FFFFFF` |
| Section title | "CASA E DECORAÇÃO" (or category name) |
| Title font | Bold, sans-serif, ~14px |
| Title color | `#222222` |
| Layout | Horizontal scroll row |
| Cards per view | 2–3 visible |
| Card width | ~100–120px |
| Card height | ~130px |
| Card background | Light grey `#F5F5F5` |
| Card border-radius | ~8px |
| Category image | Fills top ~70% of card |
| Category label | Bottom of card, centered, ~11px |
| Label color | `#333333` |
| Gap between cards | ~8px |
| Padding horizontal | ~10px |

---

## 7. Brands Section ("MARCAS")
Node: `302:1347` area (within mobile page ~y=2003)

| Property | Value |
|----------|-------|
| Width | 360px |
| Height | ~185px |
| Background | `#FFFFFF` |
| Section title | "MARCAS" |
| Title font | Bold, ~14px |
| Title color | `#222222` |
| Brand logos | Horizontal carousel, ~3 visible at once |
| Logo container | Rounded square, ~143 × 143px |
| Logo background | White |
| Logo size | ~80–100px wide |
| Carousel arrows | Magenta chevrons |
| Gap | ~10px |

---

## 8. Seasonal Banners / Promotional Banners
Node: within `1:265` (visible in full page screenshot between product shelves)

| Property | Value |
|----------|-------|
| Width | 360px |
| Height | ~160–200px per banner |
| Background | Various (image backgrounds) |
| Badge text | "30% off", "25% off" (white text on semi-transparent overlay) |
| Badge background | Dark semi-transparent overlay |
| Layout | Full-width image banners |
| Border-radius | 0 (full bleed) |
| CTA | None visible or subtle |
| Stacking | 2 banners side-by-side (each ~175px wide) or full-width |

---

## 9. About Us Section ("SOBRE A UPNEXT")
Node: `302:1378` — `sobre upnext` (340 × 983px, y=2725)

| Property | Value |
|----------|-------|
| Width | 340px (10px padding each side) |
| Height | 983px (expanded accordion) |
| Background | `#FFFFFF` |
| Section title | "SOBRE A UPNEXT" |
| Title font | Bold, sans-serif |
| Title size | ~18px |
| Title color | `#222222` |
| Title accent | Magenta `#8C1A47` icon/bar before title |
| Phone mockup image | ~200 × 300px, centered, shows UpNext app |
| Phone image bg | Magenta blob shape behind phone |
| Body text | Multi-paragraph, ~14px, dark grey `#333333` |
| Body line-height | ~1.6 |
| Body font | Regular, sans-serif |
| Layout | Stacked column (phone image then text below) |
| Arrow | Small ">" magenta arrow after title (accordion toggle) |
| Padding | 10px horizontal |

---

## 10. Newsletter Section
Node: `1:392` — `newsletter` (360 × 283px)

| Property | Value |
|----------|-------|
| Width | 360px |
| Height | 283px |
| Background | `#2C2C2C` (dark charcoal/near-black) |
| Icon | House/newsletter icon, magenta `#8C1A47`, ~40px |
| Title | "ASSINE NOSSA NEWSLETTER" |
| Title font | Bold, all-caps |
| Title size | ~20px |
| Title color | `#FFFFFF` |
| Title line-height | 1.2 |
| Input "Nome" | Full-width minus padding, bottom border only |
| Input "Email" | Full-width minus padding, bottom border only |
| Input background | Transparent |
| Input text color | `#FFFFFF` (placeholder text) |
| Input border | Bottom line `#555555` or similar |
| Input height | ~40px |
| CTA button | "ENVIAR", full width, magenta `#8C1A47` background |
| CTA height | ~38px |
| CTA font | Bold, ~14px, white |
| CTA border-radius | ~4px |
| Privacy text | ~10px, grey `#AAAAAA`, below button |
| Padding horizontal | ~10px |
| Gap between fields | ~10px |
| Layout | Column |

---

## 11. Footer (Rodapé)
Node: `1:283` — `rodape` (360 × 1462px)

### 11a. Model/About image area
| Property | Value |
|----------|-------|
| Background | `#F5F5F5` (light grey) |
| Image | Woman in yellow shirt, holding UpNext branded sign |
| Image size | ~132 × 210px |
| Image position | Centered |
| About text | Body text, ~13px, dark `#333333` |
| Padding | ~10px horizontal |

### 11b. Accordion sections
| Property | Value |
|----------|-------|
| Background | `#F5F5F5` |
| Section titles | "AJUDA E SUPORTE", "MINHA CONTA" |
| Title font | Bold, ~14px |
| Title color | `#222222` |
| Divider | Thin line `#DDDDDD` between sections |
| Arrow icon | Chevron, magenta `#8C1A47`, rotates on expand |
| Padding horizontal | ~10px |
| Section height (collapsed) | ~50px |

### 11c. Customer Service (Atendimento SAC)
| Property | Value |
|----------|-------|
| Background | `#F5F5F5` |
| Label | "ATENDIMENTO SAC" bold ~13px |
| Sub-label | "Dúvidas sobre produtos e serviço de entrega?" |
| Contact icons | Phone, WhatsApp, Email — magenta `#8C1A47`, ~40px each |
| Icon container | Circle, white background |
| Hours text | "Seg a Sex: 8h às 23h59. Sáb e Dom: 9h às 15h..." |
| Hours font | ~12px, grey |
| Icons spacing | ~30px between icons |

### 11d. Payment Methods
| Property | Value |
|----------|-------|
| Label | "PAGAMENTO" |
| Icons | Visa, Mastercard, Elo, Amex, Hiper, Boleto, PIX |
| Icon size | ~32 × 20px each |
| Icons layout | Row, left-aligned |
| Padding | ~10px |

### 11e. Social Media Icons
| Property | Value |
|----------|-------|
| Icons | Facebook, Instagram, LinkedIn, YouTube |
| Icon size | ~32px |
| Icon color | Dark grey / original brand colors |
| Layout | Row, centered |
| Gap | ~12px |

### 11f. Legal / Copyright
| Property | Value |
|----------|-------|
| Text | "© 2023 Copyright – UPNEXT – Todos os direitos reservados. R. Buenos Aires, 73 Batel, Curitiba – PR" |
| Font size | ~11px |
| Color | `#555555` |
| Layout | Center-aligned |

### 11g. Trust Badges
| Property | Value |
|----------|-------|
| Badges | "Google Safe Browsing", "Let's Encrypt" |
| Badge size | ~130px wide each |
| Layout | Row, centered |
| Gap | ~20px |

### 11h. Footer Logo Bar
| Property | Value |
|----------|-------|
| Background | `#FFFFFF` |
| Logos | UpNext logo (dark) + VTEX logo |
| Logo size | ~99 × 30px (UpNext), ~85 × 20px (VTEX) |
| Layout | Row, centered |
| Gap | ~30px |
| Padding | ~20px vertical |

---

## 12. Mobile Drawer / Category Menu
Node: `2744:476` parent — `topo` (360 × 63px header + drawer overlay)

| Property | Value |
|----------|-------|
| Hamburger icon | White 3-line icon, far right of header |
| Hamburger icon size | ~22 × 16px |
| Drawer background | `#8C1A47` (dark magenta) |
| Drawer width | 100% or ~280px slide-in from left |
| Close button | X icon, top right |
| Menu items | Links in white, ~16px, regular |
| Menu padding | ~20px horizontal |

---

## Global Mobile Tokens

| Token | Value |
|-------|-------|
| Primary color | `#8C1A47` (dark magenta/maroon) |
| Accent/CTA green | `#27AE60` |
| Background (page) | `#FFFFFF` |
| Background (sections) | `#F5F5F5` |
| Background (dark sections) | `#2C2C2C` |
| Text primary | `#222222` |
| Text secondary | `#555555` |
| Text light | `#888888` |
| Text on dark | `#FFFFFF` |
| Font family | Inter (or similar geometric sans-serif) |
| Base font size | 14px |
| Frame width | 360px |
| Horizontal padding | 10px |
| Border radius (cards) | 4–8px |
| Border radius (buttons) | 4px |
| CTA button height | 38–40px |

---

## Section Layout — Vertical Stack Order (top to bottom)

| # | Section | Node | Y Position | Height |
|---|---------|------|------------|--------|
| 1 | Info bar (frete grátis) | `2741:8` | 0 | 29px |
| 2 | Header (logo + icons) | `2808:233` | 29 | 63px |
| 3 | Hero banner | `1:266` | 92 | ~404px |
| 4 | Benefits bar | within `1:265` | ~496 | ~80px |
| 5 | RESTOFF countdown | within `1:265` | ~576 | ~60px |
| 6 | Product shelf "Super Ofertas" | `2727:55` | ~444 | ~520px |
| 7 | Category cards | within `1:265` | ~1400 | ~200px |
| 8 | Product shelf #2 | within `1:265` | ~1600 | ~500px |
| 9 | Brands section | within `1:265` | ~2003 | ~185px |
| 10 | Product shelf #3 | within `1:265` | ~2185 | ~500px |
| 11 | Seasonal banners | within `1:265` | ~2700 | ~300px |
| 12 | About Us | `302:1378` | 2725 | 983px |
| 13 | Newsletter | `1:392` | 3715 | 283px |
| 14 | Footer | `1:283` | 3715 | 1462px |
| 15 | Back to top | `1:453` | 5212 | 45px |

---

## Notes for Implementation

1. **Header background**: The magenta is consistently `#8C1A47` — verify exact hex via VTEX Site Editor color variables.
2. **Font**: The design uses a geometric sans-serif (likely Inter or similar); the project already uses Inter font files per `/assets/fonts/Inter_*`.
3. **Mobile width**: All mobile frames are exactly **360px** wide (not 375px).
4. **Product cards**: 2-column grid on mobile with ~10px horizontal padding and ~8px gap.
5. **Hero banner**: Is a carousel/slider — 360×404px total, the image overflows (424px original) creating the offset split-layout effect.
6. **Newsletter & footer share the same `rodape` container** at y=3715.
7. **About Us section** on mobile is a stacked column (image then text), unlike desktop which may be side-by-side.
8. **Accordion pattern** is used in footer for "Ajuda e Suporte" and "Minha Conta" sections.
9. **CTA buttons** (Add to cart / Enviar) use green `#27AE60`, not magenta.
10. **Carousel dots**: Active dot is magenta `#8C1A47`, inactive is grey `#CCCCCC`.
