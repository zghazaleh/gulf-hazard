# Gulf Hazard Scenarios

Static build of the scenario console (single `index.html`, D3 from cdnjs, Google Fonts).

- `index.html` — the page. Edited and republished from the Claude session; do not hand-edit.
- `met.json` — Bushehr wind forecast (MET Norway / yr.no), rewritten daily by the scheduled task until 10 Nov 2026. The page reads it on load and falls back to the embedded forecast if absent.
- `obs.json` (optional) — measured readings `{updated, items:[{station,value,unit,at,source}]}`; shown in the "Measured" strip.
- `model.json` (optional) — HYSPLIT deposition grid `{run, met, issued, t_hours, unit:"Bq/m2", grid:{lon0,lat0,dlon,dlat,nx,ny}, values:[...]}`; enables the "HYSPLIT grid" mode.

Scenario tool, not an operational product. Not for operational use.
