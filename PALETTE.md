# Decarb-AI poster/slide palette

One coherent palette for Decarb-AI materials. Three roles keep it from getting
muddy: **brand** (identity), **structure** (neutral slate), and **hazard**
(semantic accents, used only for their meaning). Brand blue/cyan/green are
sampled from the official `bg-title.png` swoosh, so they match the slide deck.

## Brand core (identity — headers, tabs, sweeps)

| Role | Hex | Token | Where |
|------|-----|-------|-------|
| Brand blue | `#4366AE` | `--brand-blue` | header start, section tabs, rule start |
| Brand cyan | `#38BBEC` | `--brand-cyan` | header middle, rule fade |
| Brand green | `#82C046` | `--brand-green` | header end |
| Brand sky | `#55CBF2` | `--brand-sky` | light cyan tint for gradients |

## Structure (neutral — bars, borders, dark UI)

| Role | Hex | Token |
|------|-----|-------|
| Slate | `#46536A` | `--accent` |
| Slate deep | `#333D4F` | `--accent-deep` |
| Slate light | `#ECEFF3` | `--accent-light` |
| Slate soft | `#D9DEE6` | `--accent-soft` |

## Hazard accents (semantic only — never decorative)

Muted to sit beside Figure 1's academic palette, unlike the vivid brand. Both
pass AA (≥4.5:1) on white for bold keyword text. Drought stays a red.

| Role | Hex | Token | Meaning |
|------|-----|-------|---------|
| Drought red | `#A24438` | `--drought` | drought emphasis (dusty red, 6.1:1) |
| Drought soft | `#F4E4E1` | `--drought-soft` | drought fill |
| Flood blue | `#3A6E99` | `--flood` | flood emphasis (steel blue, 5.4:1) |
| Flood soft | `#E5EDF3` | `--flood-soft` | flood fill |

## Neutrals

| Role | Hex | Token |
|------|-----|-------|
| Text primary | `#1A1A1A` | `--text-primary` |
| Text secondary | `#555555` | `--text-secondary` |
| Text muted | `#888888` | `--text-muted` |
| White / inverse | `#FFFFFF` | `--text-inverse` |
| Page background | `#F2F3F5` | `--bg-page` |
| Card | `#FFFFFF` | `--bg-card` |
| Border soft | `#D8D8D8` | `--border-soft` |

## Drop-in CSS

```css
:root {
  /* brand */
  --brand-blue:  #4366AE;
  --brand-cyan:  #38BBEC;
  --brand-green: #82C046;
  --brand-sky:   #55CBF2;
  /* structure */
  --accent:       #46536A;
  --accent-deep:  #333D4F;
  --accent-light: #ECEFF3;
  --accent-soft:  #D9DEE6;
  /* hazard (semantic) */
  --gold: #C2601D;  --gold-soft:  #F9EDE1;
  --flood: #4C7FB5; --flood-soft: #E5EEF6;
  /* neutral */
  --text-primary: #1A1A1A; --text-secondary: #555555; --text-muted: #888888;
  --bg-page: #F2F3F5; --bg-card: #FFFFFF; --border-soft: #D8D8D8;
}
```

The signature sweep is `linear-gradient(100deg, blue 0%, cyan 52%, green 100%)`.
