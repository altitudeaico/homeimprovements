# Price catalogue

`catalogue.json` is the **price source-of-truth** for the cost epic. It lives in the
repo (not the database) on purpose: git gives free price history — every re-priced
batch is a tracked diff.

## How it fits the architecture
- **GitHub (here)** holds the catalogue — read-only reference data.
- **The app** (`/cost.html`) fetches `catalogue.json` once and holds it in memory.
  When you add a budget line you can pick a catalogue item to auto-fill unit + low/
  target/high; the line stores a `catalogue_key` and the `catalogue_version` it came from.
- **Supabase** holds what's *used* — estimates, budget lines, receipts — each carrying
  a snapshot of the price at the time, so re-pricing the catalogue never rewrites history.

## Format
```json
{
  "version": "2026-06-29",
  "currency": "GBP",
  "items": [
    { "key": "oak-slat-panel", "name": "...", "category": "...", "unit": "panel (2400×600mm)",
      "price_low": 43.5, "price_target": 51.83, "price_high": 90, "supplier": "...",
      "confidence": "high", "notes": "..." }
  ]
}
```
- `price_low` = clearance/budget · `price_target` = typical price paid · `price_high` = premium/RRP
- `key` is kebab-case and stable — budget lines reference it.
- Bump `version` (a date) whenever prices are refreshed.

## Updating
Re-price by editing items and bumping `version`, or regenerate from a batch of scraped
rows with the build script (to come). Prices are 2026 UK retail snapshots; overseas and
Marketplace figures are indicative only and should not set the target.
