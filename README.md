# Decarb-AI slide template

A LaTeX Beamer slide template in the Decarb-AI house style, for talks given
under the Innovate for Ireland Programme.

Decarb-AI is an Innovate for Ireland centre working on AI for decarbonising
Ireland, jointly funded by Taighde Éireann – Research Ireland and AIB. This
template adapts the official Decarb-AI PowerPoint and branding pack into
Beamer, so slides can be written in LaTeX (equations, figures, references)
while keeping the official look. Adapted for easier use; structure inspired by
Andrew Parnell's [`aimsir_latex_template`](https://github.com/andrewcparnell/aimsir_latex_template).

| Title slide | Definition / equation slide |
|:---:|:---:|
| ![Title slide](docs/example-title.png) | ![Definition block](docs/example-block.png) |

## Tech stack

LaTeX Beamer (16:9) with TikZ. Latin Modern fonts. Compiles with **LuaLaTeX**.

## Getting started

1. Add the brand assets to `assets/` — see [`assets/README.md`](assets/README.md).
   They are not shipped with this repo (Decarb-AI copyright).
2. Compile with LuaLaTeX:
   ```bash
   latexmk -pdflua main.tex
   ```
   (pdfLaTeX may fail on some TeX installs with a missing math-font error; use
   LuaLaTeX.)
3. Edit `main.tex`: set `\title`, `\author`, `\date`. Swap the cover photo with
   one line: `\renewcommand{\titlephoto}{assets/your-photo.jpg}`.

## What's included

- **Title slide** with logos, title/author/date, and a cover photo masked to the brand curve
- **Content slides** with a bold headline, spaced bullets, and a swoosh footer showing the name and `x/total` page number
- **Definition/equation block**, a tinted panel for a key equation
- **Conclusions**, a closing slide set apart by a faint wash with the funders repeated (no "thank you" slide)
- **References** with hanging indents that break across pages for long lists
- **Acknowledgement** and **backup/appendix** slides

## Project structure

```
beamerthemedecarb.sty   the theme (palette, layouts, title/conclusions/footer)
main.tex                example deck — edit this
assets/                 brand assets (gitignored; see assets/README.md)
docs/                   README example images
```

## Licence

Template code: MIT (see [`LICENSE`](LICENSE)). The Decarb-AI brand assets are
excluded and remain the property of Decarb-AI / Research Ireland / AIB.
