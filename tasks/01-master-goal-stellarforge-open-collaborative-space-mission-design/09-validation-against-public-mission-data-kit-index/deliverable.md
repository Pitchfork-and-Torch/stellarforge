# Validation against public mission data + KIT-INDEX

**Task:** Validation against public mission data + KIT-INDEX  
**Package:** StellarForge Mission Design Education Kit (peaceful exploration / education only)  
**License:** MIT / Apache-2.0 (see `LICENSE`, `NOTICE`)  
**Attribution:** Forged on GrokForge (historical marketplace; sealed kit)

## Artifact footer (rails)

- Open license header matching this package (MIT / Apache-2.0).
- Provenance: cite public catalogs and archive DOIs/URLs used for each check.
- Dual-use refuse: no weapons, strike systems, reentry attack profiles, or export-controlled technical data.
- No secrets, credentials, or private home paths in artifacts.
- Retain "Forged on GrokForge" when redistributing the sealed kit.

## Problem with the prior draft (why this rewrite)

The previous accepted body validated a fictional "GrokForge leaf worker" against sea-level / plant-detection checklists and cited URLs that do not describe space-mission catalogs (`kitindex.com` leaf-detection pages; a non-existent Green Scientific agronomy article). That does not satisfy this leaf's title or the README seal target (mission-design education kit + KIT-INDEX against **public mission data**).

## Purpose

Give student / CubeSat teams a concrete, honest checklist for checking StellarForge example mission packs (CubeSat LEO, lunar ISRU concept) against **real, publicly available** mission and ephemeris data - without inventing catalogs or claiming flight heritage the kit does not have.

## KIT-INDEX (v0)  -  public sources to index

| ID | Source | What to pull | Typical use in this kit |
| --- | --- | --- | --- |
| KIT-TLE | [CelesTrak](https://celestrak.org/) NORAD TLEs / GP data | Two-line elements for educational CubeSat-class objects | Cross-check orbital period / inclination bands used in example LEO packs |
| KIT-SPICE | [NAIF SPICE](https://naif.jpl.nasa.gov/naif/) kernels + tutorials | Planetary constants, ephemerides (public kernels only) | Multi-body sketch validation limits for classroom sims |
| KIT-NASA-SSD | [NASA SSD / Horizons](https://ssd.jpl.nasa.gov/horizons/) | Ephemerides for Moon / Earth | Sanity-check lunar transfer sketch Δv order-of-magnitude |
| KIT-NSSDCA | [NASA NSSDCA](https://nssdc.gsfc.nasa.gov/) master catalog | Historical mission fact sheets | Compare payload mass / orbit class labels in example packs |
| KIT-ESA-EO | [ESA Earth Online / EO missions](https://earth.esa.int/) (public pages) | Public EO CubeSat / smallsat mission summaries | Classroom "similar class" references - not design authority |

Do **not** treat any row as ITAR/EAR technical assistance. Use only published public pages and open kernels.

## Validation plan (step-by-step)

1. **Bind each example pack to sources.** For `mission-packs` CubeSat and lunar-ISRU sketches, list which KIT-INDEX rows apply. If none apply, mark the parameter `UNVALIDATED` (do not invent a citation).
2. **Orbital class check (CubeSat LEO pack).** From KIT-TLE, pick a public educational/cubesat TLE set. Compare pack claims for altitude band, period, and inclination to the catalog ranges. Record pass / fail / out-of-scope.
3. **Δv honesty check (lunar sketch).** Using KIT-NASA-SSD public Horizons ephemerides and a textbook Hohmann/patched-conic classroom formula, verify the pack's Δv figures are within a stated educational tolerance (e.g. ±30%) **or** relabel them as illustrative only.
4. **Mass / power label check.** Against KIT-NSSDCA public fact sheets for analogous smallsat / lunar-precursor concepts, flag any pack number that exceeds published class envelopes without a citation.
5. **Refuse list audit.** Confirm the pack and this validation note still refuse weapons, strike, reentry attack profiles, and export-controlled detail (align with LEGAL-RAILS).
6. **SEAL checklist (education kit).** Before claiming "validated":
   - [ ] Every numeric claim has a KIT-INDEX ID or is marked illustrative / unvalidated  
   - [ ] All URLs resolve to public pages (no fabricated DOIs)  
   - [ ] Dual-use refuse note present  
   - [ ] License + Forged on GrokForge attribution present  
   - [ ] No claim of flight heritage or operational certification

## Scoring (honest limits)

| Score | Meaning |
| --- | --- |
| 0 | Fabricated sources or wrong domain (e.g. plant / ocean "mission data") |
| 1 | Sources listed but no parameter-level mapping |
| 2 | Partial mapping; major Δv/orbit claims still unvalidated |
| 3 | Core orbit / Δv / mass labels mapped with tolerances stated |
| 4 | Full SEAL checklist green for the example packs in this kit |

This leaf targets score ≥ 3 for the shipped example packs. It does **not** certify flight readiness.

## References (public, verifiable)

- CelesTrak GP / TLE documentation: https://celestrak.org/NORAD/documentation/
- NAIF SPICE toolkit & public kernels: https://naif.jpl.nasa.gov/naif/
- JPL Horizons system: https://ssd.jpl.nasa.gov/horizons/
- NASA NSSDCA master catalog: https://nssdc.gsfc.nasa.gov/
- National Aeronautics and Space Act peaceful-purposes policy context (legal rails sibling leaf): 51 U.S.C. § 20102

## Out of scope

Weapons design, targeting, reentry attack profiles, classified trajectories, non-public ICD detail, and any claim that this markdown kit replaces licensed mission-assurance processes.
