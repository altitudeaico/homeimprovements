# Living Room Renovation — Master Plan

**Version 2.0 · Spine document · Single source of truth**

> **How to use this file.** This is the authoritative spine for the living-room
> renovation. It holds everything that is *stable and whole-room*: vision, palette,
> floor plan, wall register, dependencies, build order, budget rollup, and project
> context. Wall-specific detail (surveys, build guides, shopping lists, renders)
> lives in each `Wall_X/` folder and is **referenced, not duplicated**, here.
>
> **For an AI planning agent:** ingest this spine for whole-room context, then load
> the relevant `Wall_X/` file for the wall you are working on. Do not infer
> measurements — read them from the Measurement Register (§5). If a value is `TBD`,
> it has not been surveyed yet; flag it, do not invent it.

---

## 0. Status & open foundations

Two foundations must be locked before any wall's detailed sections are trustworthy:

| Foundation | State | Blocks |
|---|---|---|
| Dining-half wall letters (A, B, C) | **PROVISIONAL** — needs owner confirmation | Floor plan labels, Wall A/B/C sections |
| Measurement Register (§5) | **MOSTLY BLANK** — survey not done | All build, board, cut, shopping tasks |

Everything else below (vision, palette, geometry shape, methodology, Wall F content)
is confirmed and stable.

---

## 1. Executive Vision

**Transform the living room into a warm, contemporary family space while respecting
the home's original character.**

### Design philosophy
Every decision must satisfy four tests, in priority order when they conflict:
1. Improve functionality.
2. Increase visual quality.
3. Remain achievable by DIY.
4. Respect the character of the house.

**When "modern" and "character" conflict, character wins.**

### Colour palette
- **Walls (primary):** deep olive green — *Farrow & Ball Studio Green No.93* (the "Bantry/Studio Green" direction). Near-black green; moody, classic, warm.
- **Joinery / cabinetry:** black (sideboard-style lower units; reeded/fluted door faces).
- **Accents / hardware:** brushed brass / gold.
- **Natural material:** oak (shelving, accents) — medium-dark tone.
- **Trim / ceiling:** kept light to frame the dark walls; smooth finish.

### Lighting philosophy
- **Warm 3000K** throughout.
- **Layered, not flat:** concealed LED used **sparingly** (under shelves/plinths, TV recess, alcoves) — never visible strip-everywhere.
- Wall sconces for symmetry and warmth; recessed warm spots for ambient; a statement pendant per zone.
- Any LED tied into a fixed circuit = electrician.

### Materials palette
Oak (shelves/accents) · black-painted MDF & reeded/fluted panels (cabinet faces) ·
CLS timber (framing) · plasterboard / fireline board near the fire · brass hardware ·
warm-white LED · dark-green and black paint systems.

### Furniture direction
Black-framed dining set · black / dark leather seating (Chesterfield-style in the
lounge half) · oak surfaces · symmetry where practical.

### Architectural principles
- **Symmetry** wherever practical (alcoves mirror each other).
- **Hidden storage** designed in, not bolted on.
- **Preserve original features:** the exposed-brick archway, the leaded diamond
  front window, and the chimney breast are kept and made into features.
- **Detailed planning before building.** No construction begins on a wall until that
  wall's mini-project documentation is complete.

---

## 2. Living Room Overview

### Floor plan (verified geometry)

One through-lounge (two original receptions knocked into one), **constant width 3.18 m**,
divided by an exposed-brick archway. Kitchen and conservatory open off the dining
half; the front lounge holds the chimney breast and the leaded front window.

```
   ← FRONT (street)                                  BACK (garden) →

 CHIMNEY SIDE   fireplace + TV (F)        fridge · kitchen door · column · HATCH (B?)
              ┌────────────────┬──────────────────────────────────┐
   leaded     │                │                                  │
   window  G ─┤   FRONT LOUNGE )  brick   DINING HALF             ├─ patio
   + curtains │                )  arch                            │  doors (D)
              │                )  A / E                           │  → conservatory
 HALL SIDE    │ door + sofa (H)│         two hall doors (C?)      │
              └────────────────┴──────────────────────────────────┘
                3.18 × depth(TBD)          3.18 × 3.44 m
```

**Dimensions:** width is constant at **3180 mm** (set by the shared divider).
Dining half depth **3440 mm** (measured). Lounge depth **TBD** — *note: the lounge
depth is the same dimension as "Wall F overall width," so surveying Wall F closes it.*
Ceiling height **TBD** (identical for every wall once measured once).

### Wall register (A–H)

Eight wall *faces*; the divider contributes one face to each room (A = dining side,
E = lounge side). **D, E, F, G, H are confirmed; A, B, C are provisional.**

| Wall | Physical face | Key features | Length | Status | Confidence |
|---|---|---|---|---|---|
| **A** | Divider — dining side | brick arch, brass sconces | 3180 | Concept | *provisional* |
| **B** | Dining kitchen wall | fridge, kitchen door, chimney column, serving hatch | 3440 | Concept | *provisional* |
| **C** | Dining hall-doors wall | two white panel doors | 3440 | Concept | *provisional* |
| **D** | Dining garden wall | patio doors → conservatory; curtains | 3180 | Approved | high |
| **E** | Divider — lounge side | brick arch, brass sconces | 3180 | Approved | high |
| **F** | Lounge **media wall** | chimney breast, fire, TV, 2 alcoves | ~3200 (TBD) | **Reference · documented** | high |
| **G** | Lounge front window | leaded diamond window; curtains | 3180 | Approved | high |
| **H** | Lounge door wall | hall door, black sofa, artwork | depth (TBD) | Approved | high |

> **Action:** confirm or correct A, B, C (which of: dining arch-face / kitchen wall /
> hall-doors wall maps to which letter). The provisional mapping above is the working
> assumption until then.

### Dependencies between walls

- **Global colour lock:** Studio Green No.93 must be confirmed before *any* wall is painted (consistency).
- **Ceiling & skim** (if walls are skimmed smooth) precede final wall paint everywhere.
- **Floor decision** (refinish existing vs replace + match) affects skirting on every wall and is best resolved before second-fix.
- **Shared divider:** A (dining face) and E (lounge face) are **one physical wall** — finish both faces in the same pass.
- **Floor continuity:** the oak floor runs across the arch through F/H/B — lay/refinish as one continuous plane.
- **Fire model choice** gates the Wall F aperture cut (do not cut before the fire is bought — see Wall F workbook R008).
- **Measurements gate everything** structural (§5).

### Recommended build order (DIY, keep room usable)

1. **Phase 0 — Whole-room survey:** photos, measurements (§5), confirm A/B/C, lock fire model, finalise renders. *Gate: no build until complete.*
2. **Wall F (media wall)** — the dust-heavy structural build and the methodology prototype. Prove the process here.
3. **Any other "build" walls** (e.g., joinery on the kitchen-wall side, if scoped) while construction tolerance is high.
4. **Second-fix:** door swaps, curtain tracks/hardware, brass.
5. **Ceiling/skim → whole-room paint pass** (Studio Green + black joinery) in one go for even colour and fewer cut-ins.
6. **Flooring** (refinish or lay) once messy work is done; then skirting.
7. **LED + fixed electrics** (electrician where required).
8. **Styling → snagging** room-wide.

*Order is adjustable; the hard rules are the dependencies above.*

### Budget summary

| Scope | Low £ | Target £ | High £ | Notes |
|---|---|---|---|---|
| **Wall F (media wall)** | 1,974 | 3,753 | 7,159 | From Wall F workbook; DIY labour excluded |
| Walls A, B, C, D, E, G, H | TBD | TBD | TBD | Mostly paint / curtains / door / decor — far cheaper per wall than F |
| **Whole-room (rough order)** | ~4,000 | ~6,000–8,000 | ~12,000+ | Materials only, DIY; **verify all prices locally** |

Wall F is the expensive outlier (the only full build). Carry a **running total** and a
must-have-vs-later split to control creep (Wall F workbook R006).

### Timeline summary
Wall F alone is scoped at ~7 phases across ~3 months of weekends (Wall F workbook
*Schedule* sheet). Remaining walls are mostly decoration and schedule faster once
F has proven the method.

---

## 3. Methodology

Every wall is an independent mini-project containing: Survey · Design · Execution ·
Procurement · Planning · Documentation. **Wall F is the prototype** — once fully
documented and built, the same 16-section structure (see `WALL_TEMPLATE.md`) is applied
to every remaining wall until the whole room has a professional renovation manual.

Master workflow:
`Survey → Design → Render → Review → Decompose into mini-projects → IKEA-style build manuals → Cost → Shopping list → Schedule → Build → Review → Refine.`

---

## 4. Wall sections (index)

Each links to its folder. Detail lives there, not here.

- `Wall_A/` — divider, dining side. *Concept; awaiting confirmation + decomposition.*
- `Wall_B/` — dining kitchen wall. *Concept; awaiting confirmation + decomposition.*
- `Wall_C/` — dining hall-doors wall. *Concept; awaiting confirmation + decomposition.*
- `Wall_D/` — dining garden wall. *Approved; window-treatment spec pending.*
- `Wall_E/` — divider, lounge side. *Approved; decorating + lighting spec pending.*
- `Wall_F/` — **media wall.** Reference implementation. Design + all six build manuals
  complete (`Wall_F.md` + `manuals/`): master elevation (two variants A/B), remove,
  corbel removal, expose, build frame, board & finish, cut opening, install fire.
  *Pending: variant choice, on-site survey, budget/procurement/schedule.*
  *(See `Wall_F.md` and `Wall_F_Renovation_Planning_Workbook.xlsx`.)*
- `Wall_G/` — lounge front window. *Approved; curtain spec pending.*
- `Wall_H/` — lounge door wall. *Approved; door + artwork refinements pending.*

---

## 5. Measurement Register (master survey)

> The single most important table to fill. Every build task reads from here.
> Survey once; values propagate to all wall docs. `TBD` = not yet measured.

| Ref | Area | Measurement | Value (mm) | Confirmed |
|---|---|---|---|---|
| M01 | Whole room | Ceiling height | TBD | No |
| M02 | Whole room | Width (constant, set by divider) | 3180 | Yes (owner) |
| M03 | Dining half | Depth (walls B & C length) | 3440 | Yes (owner) |
| M04 | Lounge | Depth (walls F & H length = Wall F overall width) | ~3200* | from elevation |
| M05 | Divider | Brick arch — width | TBD | No |
| M06 | Divider | Brick arch — height to apex | TBD | No |
| M07 | Divider | Brick arch — offset from corner | TBD | No |
| M08 | Wall B | Kitchen doorway — width + offset | TBD | No |
| M09 | Wall B | Serving hatch — width + sill height + offset | TBD | No |
| M10 | Wall C | Hall door 1 — width + offset | TBD | No |
| M11 | Wall C | Hall door 2 — width + offset | TBD | No |
| M12 | Wall D | Patio doors — width + height + offset | TBD | No |
| M13 | Wall F | Chimney breast — width + projection (depth) | TBD | No |
| M14 | Wall F | Chimney opening — W × H × D | TBD | No |
| M15 | Wall F | Left + right alcove — width + depth | TBD | No |
| M16 | Wall G | Front window — W × H + sill + offset; flat or shallow bay? | TBD | No |
| M17 | Wall H | Hall door — width + offset | TBD | No |

*(Wall F's internal survey detail also lives in its workbook Measurements sheet; M13–M15 mirror it.)*

---

## 6. Procurement

- **Master shopping list:** roll-up of per-wall lists. Wall F's is complete in its
  workbook; other walls' lists are produced as each is decomposed.
- **Suppliers (observed):** Wickes (CLS timber), B&Q (MDF, plasterboard/fireline),
  Screwfix/Toolstation (fixings, electric fires), IKEA/B&Q (cabinet bases/doors).
  *All prices are planning allowances — verify locally before buying.*
- **Cost tracker:** maintain committed vs remaining against the §2 budget; log receipts.

---

## 7. Project management

- **Build order / dependencies:** §2.
- **Cadence:** weekend-based, single-wall focus to keep the room usable (Wall F workbook R007).
- **Cash-flow:** stage purchases (survey/tools → frame/board → fire/paint/finish) so spend lands with progress.
- **Progress tracker & snagging:** per wall, rolled up here.

---

## 8. AI context (continuity log)

### Decisions made
- Palette locked to **Studio Green No.93 + oak + black + brass + 3000K** (this *supersedes* an earlier charcoal / 2700K placeholder).
- **Keep the brick archway raw** as the hero feature — not painted or clad.
- **Keep the leaded diamond front window** as a character feature; refresh only the dressing.
- **Continuous medium-dark oak floor** across both halves and through the arch.
- **Media wall (F):** new 47×70 CLS frame in front of the chimney (chimney opening kept clear at the bottom); linear electric fire (Evonic e1800 example, ventilated); TV centred; two mirrored alcoves — 40mm oak shelves over push-to-open cabinets; brass sconces flanking the TV; 3000K LED. Design dims: 3200 W × 1550 H × 450 D; modules 800/1600/800.
- **Modular per-wall mini-project method;** Wall F is the prototype.
- **DIY-first;** professional only where required (e.g., fixed-circuit electrical).

### Decisions rejected / superseded
- Charcoal walls / 2700K lighting → replaced by Studio Green / 3000K.

### Principles to preserve
- Character beats modern in a conflict · symmetry where practical · hidden storage ·
  keep original features (arch, leaded window, chimney breast) · LED sparing and concealed.

### Open questions
- Confirm dining-half letters **A / B / C**.
- **Lounge depth**, **ceiling height**, and **all opening dimensions** (Register §5).
- **Floor:** refinish existing lounge boards vs replace + match throughout.
- **Front window:** flat or shallow bay?
- **Exact electric fire model** (gates the Wall F aperture).
- **Wall F variant:** choose A (modern oak-slatted/fluted) or B (traditional shaker).
- **Lounge depth ≈3200** is inferred from the Wall F elevation — confirm on site (M04).
- Any wall besides F that warrants a full *build* vs decoration-only.

### Future enhancements
- Extend the same methodology to Kitchen, Hallway, Bedrooms (per repo structure).
- Full AI render set per wall.
- Live price tracking during procurement.

---

## 9. Changelog
- **v2.0** — Restructured as indexing spine. Added verified floor plan, A–H register
  with confidence flags, dependency matrix, build order, budget rollup, master
  Measurement Register, AI-context log. Palette corrected to Studio Green / 3000K.
- **v1.0** — Initial vision, repository structure, wall register stubs.
