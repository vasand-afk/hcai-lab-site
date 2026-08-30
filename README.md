# MDAIRX

Marketing/portfolio site for **Dr. Vasan's ℞ for HealthCare facilities** —
physician-led diagnostic and workflow AI across clinical imaging and care
operations.

Static single-page site, no build step. `index.html` is self-contained:
all CSS and JS are inline, and the platform/solution cards are rendered
from a data array near the bottom of the file.

## Structure

| Section | Purpose |
|---|---|
| Platforms | The two general-purpose systems everything else plugs into |
| Solutions | The nineteen clinical models, filterable by domain |
| Facilities / Insurers / Investors | Audience-specific pages |
| Careers, Contact | — |

## Editing the cards

Both grids are driven by the single `PROJECTS` array. An entry with
`domain:"platform"` renders into the Platforms section; everything else
renders into Solutions, grouped by `label` and filtered by `domain`.
