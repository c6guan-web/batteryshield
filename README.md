# Battery Shield

Landing page and technical datasheet for **Battery Shield** — a passive, AI-discovered
1.5 mm phase-change material that integrates heating, cooling, insulation and fire
suppression in a single layer, stopping lithium-ion thermal runaway before it spreads.

## Contents

| Path | Description |
|------|-------------|
| `index.html` | Single-page marketing site (English, dark-gray / green tech style). Open directly in a browser. |
| `assets/logo.jpg` | Battery Shield logo |
| `assets/experiment.png` | Live overcharge-test photo with temperature overlay |
| `assets/{yang,guan,khor,alessandro}.{jpg,png}` | Team headshots used in the site |
| `datasheet/BatteryShield_说明书.tex` | LaTeX source of the Chinese technical spec / 详细功能说明 |
| `datasheet/BatteryShield_说明书.pdf` | Compiled Chinese PDF spec (6 pages) |

## View the site

Open `index.html` in any modern browser — no build step or server required.

## Rebuild the datasheet PDF (Chinese — needs XeLaTeX)

```bash
cd datasheet
xelatex BatteryShield_说明书.tex   # run twice (pgfplots/refs)
xelatex BatteryShield_说明书.tex
```

Requires a TeX distribution with `ctex`, `pgfplots`, `booktabs`, `tabularx`, `multicol`
and `hyperref`, plus a CJK font (e.g. TeX Live 2025 on Windows uses the system fonts).

---

*Figures are drawn from the project's internal business plan, laboratory open-test data
and industry-expert interviews, and are indicative pending independent third-party
certification. "GB 38031" is the Chinese national standard for EV battery safety.*
