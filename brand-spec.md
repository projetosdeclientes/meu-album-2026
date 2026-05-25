# Meu Álbum 2026 — Brand spec

## Visual territory
Panini / FIFA sticker album meets premium sportswear. Clean paper-white canvas
with Brazil's national palette — green field, yellow gold, deep blue sky.
The sticker card is the atomic design unit: vertical 3:4 ratio, blue premium
border, green/yellow field, number 26 watermark, Brazil flag, "BRA" vertical
text, name, age, team, Seleção jersey. Ultra-realist portrait style.

## Color tokens

```css
:root {
  --bg:      oklch(97.5% 0.004 90);   /* warm paper — album page */
  --surface: oklch(100% 0 0);          /* card white */
  --fg:      oklch(16% 0.03 250);      /* deep navy */
  --muted:   oklch(45% 0.025 240);     /* slate */
  --border:  oklch(86% 0.015 230);     /* light blue-grey */
  --accent:  oklch(48% 0.18 255);      /* Brazil blue #002776 */
  --green:   oklch(50% 0.20 140);      /* Brazil green #009739 */
  --yellow:  oklch(84% 0.18 90);       /* Brazil gold #FEDD00 */
  --gold:    oklch(70% 0.14 80);       /* premium gold accent */
}
```

- Blue is the primary accent (buttons, borders, eyebrow).
- Green is the secondary field (backgrounds, decorative panels).
- Yellow is the tertiary spark (badges, highlights, stars).
- Gold is the premium upgrade signal (holographic, gold edition).

## Typography

- **Display:** `'Inter', 'Segoe UI', -apple-system, system-ui, sans-serif`
  Bold, condensed feel. FIFA / Panini use blocky sans for names.
- **Body:** `-apple-system, BlinkMacSystemFont, 'Segoe UI', system-ui, sans-serif`
- **Mono:** `ui-monospace, 'JetBrains Mono', Menlo, monospace` (for numbers, age)

No serif unless a quote needs it. This is sport, not editorial.

## Posture rules

1. **Sticker card = hero unit.** Every visual section should feel like flipping
   through an album page — bordered cards, clean grids, paper-white gutters.
2. **One decisive 3D element.** The hero banner gets a floating sticker card
   with CSS 3D perspective tilt. No other 3D on the page.
3. **Accent budget per screen:**
   - Blue accent: max 2× per screen (eyebrow + primary CTA)
   - Green: max 1 decorative panel per screen
   - Yellow: badges or highlights only — never a page wash
4. **No rounded boxes with left-border accent.** (Classic AI-slop trope.)
   Instead use full card borders in blue or a full surface tint.
5. **Monoline SVGs only.** No emoji as feature icons. Football ⚽ emoji is
   allowed in headings and CTAs since it's the product symbol.
6. **Real copy, no filler.** Every Portuguese phrase is specific: club names,
   prices, WhatsApp message templates.
7. **WhatsApp green (#25D366) for all WhatsApp buttons**, not the accent blue.
   WhatsApp buttons must be recognizable at a glance.
