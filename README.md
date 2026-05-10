# WBGT Heat Stress Calculator

A lightweight, single-file web calculator that estimates **Wet Bulb Globe Temperature (WBGT)** using the Epstein formula. No dependencies, no build tools — just one HTML file.

## Live Site

👉 [itoshmi.github.io/heat-stress-wbgt](https://itoshmi.github.io/heat-stress-wbgt.github.io/)

👉 [heatstress.org](https://heatstress.org/)

## What it does

Calculates WBGT from:
- Air temperature (°C) — matrix rows/columns
- Relative humidity (%) — matrix rows/columns
- Cloud cover (%) — adjustable slider
- Atmospheric pressure (hPa) — adjustable slider

Results are color-coded by risk level:

| Color | Range | Level |
|---|---|---|
| 🟢 Green | < 25 | Normal |
| 🟡 Yellow | 25 – 27.9 | Caution |
| 🟠 Orange | 28 – 29.4 | Extreme Caution |
| 🔴 Light red | 29.5 – 31.9 | Danger |
| 🔴 Red | ≥ 32 | Extreme Danger |

## Languages

Supports 🇺🇸 English, 🇲🇽 Spanish, 🇧🇷 Portuguese, 🇫🇷 French — switchable via flag buttons.

## Formula

Based on the **Epstein simplified WBGT formula**:

```
WBGT = 0.567·T + 0.393·Pv + 3.94·(1 − cloud/100)
Pv   = (RH/100) · 6.105 · e^(17.27·T / (237.7+T)) · (P/1013.25)
```

Reference: Prof. Yoram Epstein — Ariel hiking heat stress guidelines.

## Files

```
index.html   # The entire app — calculator, styles, and logic
README.md    # This file
```

## Usage

Open `index.html` in any modern browser. No installation or internet connection required.
