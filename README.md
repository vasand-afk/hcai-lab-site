# MDAIRX

Marketing/portfolio site for **MDAIRX** — Dr. Vasan's AI Rx for HealthCare
facilities. Physician-led diagnostic and workflow AI across clinical
imaging and care operations.

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

## The Rx mark

The prescription symbol in the wordmark and hero is composed in CSS —
an `R` with a smaller `x` positioned over its descending leg — rather
than the Unicode glyph U+211E, whose rendering varies by font and is
absent from several common stacks. The markup carries `aria-label="Rx"`
so screen readers announce it correctly.
