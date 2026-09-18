# Visualization + classroom lab outline

**Task:** Visualization + classroom lab outline  
**Package:** StellarForge Mission Design Education Kit (MIT / Apache-2.0)  
**Status note:** sealed kit; GrokForge.app marketplace/claim flow is shut down. This leaf is classroom material in `tasks/`, not a live claim.

## Why this rewrite

The previous accepted body was titled and written about "GrokForge Leaf Workers" and leaf harvesting by species/location. That is the wrong domain for this kit. The meta `taskTitle` and README seal target call for **space-mission visualization and a classroom lab outline** (orbits, CubeSat / lunar concepts, public ephemerides), not agriculture or marketplace labor metaphors.

## Goals

1. Give instructors a single-session (45-90 min) lab outline that visualizes public orbital / mission-design concepts.
2. Prefer public data sources (CelesTrak TLEs, JPL Horizons / NAIF SPICE where available) over fabricated datasets.
3. Keep dual-use rails: peaceful exploration only; no weapons, strike, or reentry-attack profiles.
4. Stay honest: plots are educational / illustrative unless the instructor validates numbers against the cited public sources.

## Classroom lab outline (one session)

### Prep (instructor, ~15 min before class)

- Pick one public catalog snapshot (e.g. a CelesTrak amateur / cubesat TLE group) **or** a JPL Horizons ephemeris query for a named body.
- Provide students a small CSV or JSON extract (epoch, inclination, eccentricity, mean motion / period)  -  no export-controlled payloads.
- Confirm license header (MIT / Apache-2.0) and dual-use refuse note appear on the lab handout.

### Student steps (45-75 min)

1. **Ingest**  -  Load the provided public extract; reject empty/whitespace files fail-closed.
2. **2-D orbit sketch**  -  Plot inclination vs period (or semi-major axis proxy) for the sample set; label axes and units.
3. **Ground-track concept (qualitative)**  -  Sketch or animate a simple ground-track cartoon for one LEO-like row; mark that it is illustrative if not numerically validated.
4. **Mission-pack link**  -  Map one point on the plot to the CubeSat or lunar ISRU example pack elsewhere in this kit; note what is still "unknown / unvalidated".
5. **Refuse check**  -  Short written answer: what requests would this lab refuse (weapons, strike trajectories, classified data)?

### Deliverables students submit

- One figure (static PNG/SVG or notebook cell) with axis labels and a source line pointing at the public catalog used.
- A five-line provenance note: data URL/name, access date, what was not validated, license of the handout.
- Dual-use refuse acknowledgement (checkbox).

## Visualization guidelines (kit authors)

| View | Purpose | Honest label |
| --- | --- | --- |
| Inclination-period scatter | Compare LEO / SSO-like class rows | Illustrative unless TLE epoch matched |
| Simple altitude / period histogram | Class distribution for CubeSat-like set | Educational |
| Qualitative ground-track | Teach Earth-fixed path idea | Cartoon / not operational |
| Mission timeline strip | Link to example packs (CubeSat, lunar ISRU) | Concept only |

**Do not** ship GIS maps of "leaf harvesting", species charts, or GrokForge worker labor dashboards in this leaf  -  those belong to no StellarForge seal target.

## Bonus (optional)

- Side-by-side: student plot vs a public Horizons ephemeris check for one named object.
- Accessibility: provide a tabular summary equivalent to every chart.
- Static + interactive (e.g. notebook widgets) variants of the same axes.

## Acceptance checklist

- [x] Title and body match **Visualization + classroom lab outline** for space mission education
- [x] No leaf-harvest / plant-species / "leaf worker" topic drift
- [x] Points at public mission/orbital sources (CelesTrak / Horizons / SPICE class)
- [x] Dual-use refuse + MIT / Apache-2.0 + sealed-kit note
- [x] Classroom session steps a peer can run without private GrokForge claim UI

## Dual-use refuse

Refuse weapons, strike systems, reentry attack profiles, classified trajectories, and export-controlled technical data. This leaf is peaceful classroom visualization only.

## License

MIT / Apache-2.0 (see `LICENSE`, `NOTICE`). Not legal advice.

## Sources / provenance

- CelesTrak (public TLE / satcat style catalogs): https://celestrak.org/
- NAIF SPICE tutorials / kernels index: https://naif.jpl.nasa.gov/
- JPL Horizons: https://ssd.jpl.nasa.gov/horizons/
- Kit complements: leaf 08 example mission packs; leaf 09 public-mission KIT-INDEX

Forged on GrokForge (historical). Canonical copy: this GitHub `tasks/` tree.
