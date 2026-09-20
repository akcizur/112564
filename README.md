# Botanic Operations

Twenty-style inventory / operations UI customized for the Botanic sklad workflow.

## Model

```text
Surovina
   ↓
 Pack
   ↓
 Box
   ↓
Pozice
```

Critical rule: **one Box has exactly one Pozice**. Packs inherit their displayed Pozice from their current Box.

## UI

- Dashboard
- Packy
- Boxy
- Pozice
- Suroviny
- Pohyby
- Historie
- Global search / `Ctrl+K` / `⌘K`
- Pack detail drawer
- Box detail drawer
- Pack move flow
- Box move flow
- New Pack flow
- Responsive desktop/mobile layout
- Light neutral design system with lime accent

## Data fields

Pack: `ID Pack`, `Surovina`, `Šarže`, `Expirace MM/YY`, `Box`, `Stav`.

Box: `ID Box`, `Pozice`.

No separate Pack position is stored in the model.

## GitHub Pages

The application is static and can be deployed from `main` / root using GitHub Pages.

Current demo data is held in `app.js`. The next integration step is replacing this local state with the Botanic Google Sheets / Apps Script API while preserving the same UI and validation model.
