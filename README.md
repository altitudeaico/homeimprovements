# Home Renovation

Master source of truth for the home renovation. DIY-first; detailed planning before building.

**Start here:** [`Living Room/MASTER_PLAN.md`](Living%20Room/MASTER_PLAN.md) — the spine document
(vision, palette, floor plan, wall register A–H, dependencies, build order, budget, measurement
register, and AI-context log).

## Structure
- `Living Room/` — active. `MASTER_PLAN.md` (spine) + `WALL_TEMPLATE.md` + `Wall_A/`…`Wall_H/`.
  Wall F is the reference implementation (`Wall_F/` + workbook).
- `Kitchen/`, `Hallway/`, `Bedrooms/` — future scope, same methodology.
- `Resources/` — shared assets.

## For AI planning agents
Ingest `Living Room/MASTER_PLAN.md` first, then load only the `Wall_X/` file you are working on.
Read measurements from the Measurement Register (§5) — never invent a `TBD` value.
