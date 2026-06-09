# Planilha de Comparação — Figma vs Implementação Atual
**UpNext VTEX IO Store Theme**  
**Data:** 2026-05-27  
**Fontes:** figma-desktop.md · figma-mobile.md · page-narrow.md · page-wide.md

**Status:**
- ✅ Correto
- ⚠️ Implementado com divergência
- ❌ Não implementado / quebrado
- 🔴 Bug crítico encontrado na inspeção

---

## 1. CORES (Desktop)

| Seção | Propriedade | Figma | Atual | Status |
|-------|-------------|-------|-------|--------|
| Topbar | Background | `#3D0020` | `#591032` | ⚠️ cor diferente |
| Navbar | Background | `#8B003B` | `#910e4b` | ⚠️ cor diferente |
| Category menu | Background | `#8B003B` (igual navbar) | `#910e4b` | ⚠️ cor diferente |
| Search bar | Background interno | `#5C0030` | `#61163a` | ⚠️ cor diferente |
| Search bar | Borda | wine/maroon | `#c80d65` | ⚠️ verificar |
| "Ver Ofertas" | Background | `#F5C518` (dourado) | Não verificado | ❓ |
| About Us | Background | `#7A003A` | `#910e4b` | ⚠️ cor diferente |
| Newsletter strip | Background | gradient `#7A003A→#9B004A` | gradient implementado | ✅ |
| CADASTRAR btn | Background | `#CC0066` | `#c80d65` | ⚠️ divergência mínima |
| Newsletter input | Background | `#4A001E` | `#61163a` | ⚠️ cor diferente |
| Footer | Background | `#F5F5F5` | `#eee` | ⚠️ divergência mínima |
| COMPRAR btn | Background | `#22A851` | Verificar em vtex.add-to-cart | ❓ |
| Topbar text | Cor | `#FFFFFF` | `#FFFFFF` | ✅ |
| Navbar text | Cor | `#FFFFFF` | `#FFFFFF` | ✅ |

> ⚠️ **Nota:** As cores Figma são amostras visuais de screenshots — podem ter desvio de ±5 no hex. Para valores pixel-perfect usar "Copy CSS" nos nós: navbar `2788:1637`, topbar `2788:1638`, about-us `2788:1482`, newsletter `2788:1378`.

---

## 2. DIMENSÕES E TIPOGRAFIA (Desktop)

| Seção | Propriedade | Figma | Atual | Status |
|-------|-------------|-------|-------|--------|
| **Header — Topbar** | Altura | 35px | 36px | ⚠️ 1px diff |
| **Header — Navbar** | Altura total | 83px | 90px | ⚠️ 7px diff |
| **Header — Menu** | Altura | ~36px | Implementado | ✅ |
| **Header total** | Altura | 155px | ~162px | ⚠️ |
| **Logo** | Largura | 169px | 169px | ✅ |
| **Logo** | Altura | 51px | 51px | ✅ |
| **Search bar** | Largura | 453px | 453px (max) | ✅ |
| **Search bar** | Altura | 40px | 40px | ✅ |
| **Category menu** | Font size | ~14–15px | 16px | ⚠️ slight diff |
| **Category menu** | Gap | ~80px entre items | gap:8px (desktop) | ⚠️ verificar |
| **Hero banner** | Largura | 1440px full-bleed | 1440px | ✅ |
| **Hero banner** | Altura | 648px | auto (responsivo) | ✅ |
| **Info bar** | Altura | 70px | Implementado | ✅ |
| **Info bar** | Largura | 1388px (26px margin) | Implementado | ✅ |
| **Category cards** | Imagem | 215×181px | Implementado | ✅ |
| **Category cards** | Gap | ~46px | Implementado | ✅ |
| **Product card** | Dimensões | 280×477px | 280×477px | ✅ |
| **Product card** | Imagem | 237×238px | 237×237.635px | ✅ |
| **Product name** | Font size | ~14px | 16px (brandName) | ⚠️ 2px diff |
| **Product name** | Font family | Inter | Istok Web | ⚠️ fonte diferente |
| **Product price** | Font size | ~20–22px | A verificar | ❓ |
| **Product price** | Cor | `#8B003B` | A verificar | ❓ |
| **COMPRAR** | Largura | 131px | A verificar | ❓ |
| **COMPRAR** | Altura | 41px | A verificar | ❓ |
| **Seasonal banners** | Layout | 683px + 685px (2 cols) | 2 cols implementado | ✅ |
| **Seasonal banners** | Altura | 499px | Implementado | ✅ |
| **Seasonal 4-col** | Largura cards | 332px cada | Implementado | ✅ |
| **About Us** | Largura | 1388px | 1388px | ✅ |
| **About Us** | Texto width | 841px | 841px (max-width) | ✅ |
| **About Us** | Font size | ~14px | ~14px | ✅ |
| **Newsletter** | Altura | 117px | 117px | ✅ |
| **Newsletter** | Input width | 453px | 453px | ✅ |
| **CADASTRAR** | Dimensões | 211×40px | 211×40px | ✅ |
| **CADASTRAR** | Font family | Inter | Istok Web | ⚠️ fonte diferente |
| **CADASTRAR** | Font size | ~13–14px | 18px | ⚠️ 4–5px maior |
| **Footer** | Altura | 473px | Automático | ✅ |
| **Footer** | Background | `#F5F5F5` | `#eee` | ⚠️ |

---

## 3. MOBILE — Status vs Figma (360px)

| Seção | Figma Mobile | Status Atual |
|-------|-------------|--------------|
| Header bg | `#8C1A47` | ⚠️ atual usa `#910e4b` |
| Header height | 63px | ✅ implementado (~59px) |
| Info bar (frete grátis) | 29px, `#8B1A4A` | ❌ **não implementado** |
| Hero banner | 360×404px, split layout (text/img) | ⚠️ usa mesmo banner desktop |
| Benefits bar | ~80px, 4 items, `#F5F5F5` bg | ⚠️ implementado mas com bg diferente |
| RESTOFF countdown | 60px, timer bar com contagem regressiva | ❌ **não implementado** |
| Product shelf | 2-col grid, 160×220px cards | ⚠️ shelf responsivo funciona, mas sizing pode divergir |
| Category cards | horizontal scroll, ~120px cards | ⚠️ implementado mas pode divergir |
| Brands/Marcas section | carousel de logos de marcas | ❌ **não implementado** |
| About Us | coluna: imagem phone mockup + texto | ❌ **usa layout desktop** (modelo foto) |
| Newsletter bg | `#2C2C2C` dark charcoal | ⚠️ atual usa gradient vinho |
| Newsletter CTA | "ENVIAR", cor `#8C1A47` | ⚠️ atual usa "CADASTRAR" `#c80d65` |
| Footer | accordion (Ajuda e Suporte, Minha Conta) | ❌ **usa layout desktop** (4 colunas) |
| Footer ícones sociais | row horizontal | 🔴 **bug: empilham vertical no mobile** |
| Footer contato | ícone inline com texto | 🔴 **bug: ícone em linha separada** |
| Drawer | background `#8C1A47` | ✅ implementado |

---

## 4. PROBLEMAS ENCONTRADOS NA INSPEÇÃO (Responsive)

### Mobile (320–620px) — Bugs ativos

| Prioridade | Problema | Larguras afetadas |
|-----------|---------|-------------------|
| 🔴 Alta | Social icons (Instagram/TikTok/Facebook/Blogger) empilhados em coluna vertical em vez de row | 320–620px |
| 🔴 Alta | Footer: ícones de contato (telefone/whatsapp/email) em linha separada do texto | 320–620px |
| 🟡 Média | Benefícios block: wrap muito agressivo, bloco muito alto em tela estreita | 320–420px |
| 🟡 Média | Category card images cortadas na borda direita | 320px |
| 🟡 Média | Espaço branco vazio grande antes do newsletter | 620px |
| 🟢 Baixa | "Minha Sacola" label empurra logo off-center | 320px |

### Tablet/Desktop (768–1440px) — Issues ativos

| Prioridade | Problema | Larguras afetadas |
|-----------|---------|-------------------|
| 🟡 Média | Product shelf: 2 cards por linha em 768–868px (parece esparso) — deveria ser 3? | 768–868px |
| 🟡 Média | Info bar: texto levemente comprimido | 768px |
| 🟢 Baixa | A 768px VTEX pode servir template mobile dependendo do UA do browser (iPad Safari) | 768px |

---

## 5. SEÇÕES NÃO IMPLEMENTADAS

| Seção | Referência Figma | Prioridade |
|-------|-----------------|-----------|
| Info bar "frete grátis" topo mobile | figma-mobile §1a | 🟡 Média |
| RESTOFF countdown bar | figma-mobile §4 | 🔴 Alta (feature de negócio) |
| Marcas/Brands carousel | figma-mobile §7 | 🟡 Média |
| About Us — layout mobile específico | figma-mobile §9 | 🟡 Média |
| Newsletter dark (`#2C2C2C`) no mobile | figma-mobile §10 | 🟡 Média |
| Footer accordion no mobile | figma-mobile §11 | 🟡 Média |
| Hero banner mobile (split 360×404) | figma-mobile §2 | 🟡 Média |

---

## 6. PRIORIDADE DE CORREÇÕES

### 🔴 Alta prioridade (bugs visíveis)
1. **Footer social icons** — mobile: empilham em coluna, devem ser row horizontal
2. **Footer contact icons** — mobile: ícone em linha separada do texto (misaligned)
3. **RESTOFF countdown** — feature de negócio não implementada

### 🟡 Média prioridade (divergências de design)
4. **Cores do header** — topbar `#591032`→`#3D0020`, navbar `#910e4b`→`#8B003B` (verificar exato no Figma)
5. **About Us bg** — `#910e4b`→`#7A003A`
6. **Product name font** — Istok Web → Inter (Figma usa Inter)
7. **CADASTRAR button font** — Istok Web → Inter, tamanho 18px→13–14px
8. **Product shelf** — 2-up em 768–868px: considerar se deve ir para 3-up
9. **Benefits block** — wrapping agressivo em 320px
10. **Category cards** — clipping em 320px
11. **About Us mobile** — layout diferente do Figma (phone mockup)
12. **Newsletter mobile** — bg `#2C2C2C` vs atual gradient vinho

### 🟢 Baixa prioridade (polish)
13. **Footer bg** — `#eee` vs `#F5F5F5` (praticamente igual)
14. **Topbar height** — 36px vs 35px (1px diff)
15. **Navbar height** — 90px vs 83px (7px diff)
16. **Newsletter input bg** — `#61163a` vs `#4A001E`
17. **"Minha Sacola" label** — empurra logo a 320px

---

## 7. O QUE ESTÁ CORRETO ✅

- Logo tamanho (169×51px desktop, 114px mobile)
- Product card dimensões (280×477px)
- Product image tamanho (237×237px)
- Search bar dimensões (453×40px, max)
- Newsletter CADASTRAR dimensões (211×40px)
- Newsletter input dimensões (453×40px)
- About Us texto width (841px max-width)
- Hero banner full-bleed (1440px)
- Newsletter height (117px)
- Seasonal banners 2-col layout
- Seasonal 4-col cards layout
- Header sticky (scroll fix aplicado)
- Newsletter column abaixo 960px ✅ (recém implementado)
- Header sem white stripe no tablet ✅ (recém implementado)
- Category font size 16px tablet ✅ (recém implementado)
- Sem overflow horizontal em nenhuma largura testada ✅
