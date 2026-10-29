# Flooring Scope Reference: Floor Types, Typical SOW, Standards, Tools

**Purpose.** Background reference for the AI and the interviewer when tuning `flooring-installer.md` and judging answers. It is **not** a spec.

**Order of precedence.** The project specification, then the **manufacturer's written installation instructions**, then the industry standard, then this sheet. ASTM F710 itself says it doesn't supersede manufacturer instructions.

Sources and URLs are in `sources.md` §7. Verify editions per `update-checklist.md`.

**CSI sections.** Numbers are CSI MasterFormat as listed on Sweets / 3-part specs. Subsection numbers vary by project manual, so confirm against the spec you're given. Numbers and titles 03 35 43, 09 65 16, 09 65 19, 09 67 23 confirmed per MasterFormat 2018 (checked 2026-10-29; `sources.md` §8). MasterFormat 2026 numbers: VERIFY (subscription only).

---

## 0. Floor prep (applies to every type)
**CSI sections**
- 09 05 61: common work results for flooring preparation
- 09 05 61.13: moisture vapor emission control
- 03 54 00: cast underlayment (self-leveling)

**Typical SOW**
1. **Pre-install survey.**
   - Confirm the building is enclosed and HVAC is at service conditions, per the manufacturer (often 48+ hours before, during, and after).
   - Record ambient temperature and RH.
2. **Existing-floor removal.**
   - Before disturbing old resilient tile or black mastic, **assume asbestos until tested**.
   - Follow the RFCI *Recommended Work Practices* and EPA/OSHA asbestos rules (NESHAP, 29 CFR 1926.1101).
3. **Moisture testing.**
   - **ASTM F2170:** in-situ relative humidity probes. Depth is 40% of slab thickness when drying from one side, and 20% when drying from two sides.
   - **ASTM F1869:** calcium chloride MVER, reported in lb/1,000 ft²/24 h.
     - Not for gypsum or lightweight concrete, or through coatings or patch.
   - Neither method sets a pass/fail limit. **The flooring or adhesive manufacturer's limit governs.**
   - **ASTM D4263** (plastic sheet) and **ASTM F2659** (meters) are screening only.
4. **Alkalinity.** Test pH per **ASTM F710** (pH testing is required). Compare the result to the adhesive manufacturer's range.
5. **Surface profile and cleanliness.**
   - Remove curing compounds, sealers, paint, and contaminants.
   - Profile per **ICRI 310.2R CSP 1–10**:
     - Resilient adhesives usually need a clean, sound surface (low CSP).
     - Coatings need CSP 2–5 by system. Urethane cement and MMA typically need CSP 3–5.
6. **Flatness.**
   - Measure per the spec: FF/FL per **ASTM E1155** for new slabs, or a straightedge per the manufacturer.
   - Typical manufacturer tolerances:
     - Resilient: often 3/16 in. in 10 ft.
     - Large-format tile: **any edge 15 in.+: 1/8 in. in 10 ft and 1/16 in. in 2 ft** (per ANSI A108.02 §4.1.4.3.1, as quoted by CTEF).
7. **Repair and leveling.**
   - Fill cracks and non-moving joints with patch or underlayment per **F710**.
   - **Honor moving joints:** carry them through with expansion joint covers or the manufacturer's detail.
   - Apply cementitious patch or self-leveling underlayment with the manufacturer's primer. Respect the minimum and maximum thickness and the cure or moisture time before covering.
8. **Moisture mitigation**, if readings exceed the limit: a 09 05 61.13 epoxy MVE system or a manufacturer-approved adhesive system.
9. **Acclimation** of the material and adhesive per the manufacturer.
10. Document readings with photos and a log, and get a written **substrate acceptance**. Installation is commonly treated as acceptance of the substrate. Check the spec.

**Tools:** RH probes and reader (F2170), calcium chloride kits (F1869), pH paper or meter, straightedge or F-number profiler, shot blaster, grinder with HEPA vacuum (silica Table 1), scarifier, mixing station (drill and paddle), gauge rake, spiked roller, spiked shoes, laser level.

---

## 1. Polished concrete (CSI 03 35 43; 03 35 43.13 polished and dyed)
**Typical SOW**
1. Slab assessment: hardness (Mohs), flatness, joint condition, and moisture where a dye or guard requires it.
2. Mock-up to the specified **aggregate exposure** (cream, salt-and-pepper, or large aggregate) and **gloss** (CPC levels 1–4).
3. Corrective or initial grind with metal-bond diamonds. Grit sequence depends on hardness.
4. Fill joints and cracks per the spec: semi-rigid epoxy or polyurea at control joints, after the slab has shrunk.
5. Densify (lithium, sodium, or potassium silicate).
6. Grout or slurry fill for pinholes.
7. Resin-bond polish through progressive grits.
8. Optional dye or stain.
9. Guard or sealer.
10. Burnish.
11. QC per the guide spec:
    - DOI per **ASTM D5767** and haze per **ASTM D4039**, commonly 3 tests per 1,000 SF.
    - Slip testing per the spec (e.g., ANSI A326.3 DCOF).
12. Furnish the owner's maintenance instructions.

**Standards:** ACI/ASCC **310.1** polished concrete specification; ASCC **CPC** Tradesman/Craftsman certifications; ICRI 310.2R; OSHA 1926.1153 silica.

**Tools:** planetary grinders and polishers (HTC, Husqvarna, Lavina, SASE, and similar), edgers, metal- and resin-bond diamond tooling, HEPA dust extractors, microfiber densifier applicators, a propane or battery burnisher (CO monitoring if propane), a gloss meter, and a slip meter.

**Depth:** `concrete-finisher-polisher.md`.

## 2. Grind and seal (sealed or "grind and guard" concrete)
- **CSI:** often written as a reduced-scope **03 35 43** (polishing ends after densify and guard) or a concrete sealer section. Confirm in the spec.
- **Typical SOW:**
  1. Grind to the specified exposure. Fewer grits than a polish, typically ending at about 100–200 resin.
  2. Densify.
  3. Fill the joints.
  4. Apply a penetrating sealer or topical guard (often 2 coats).
  5. Burnish if specified.
- **Standards and tools:** same as polished concrete. Gloss and DOI targets are lower or not specified.

## 3. Resinous flooring: epoxy, urethane cement, MMA (CSI 09 67 23 resinous flooring; 09 96 high-performance coatings for thin films)
**Typical SOW, common to all systems**
1. Moisture and pH testing per the manufacturer.
2. Mechanical prep (shot blast or grind) to the system's **CSP**.
3. **Pull-off adhesion test** where specified (ASTM D7234).
4. Saw-cut **keyway or anchor terminations** at the perimeter, drains, and doorways (required for urethane cement and most MMA).
5. Crack and joint detailing: honor moving joints.
6. Primer.
7. Body coat: self-leveling, trowel, broadcast, or slurry.
8. Broadcast aggregate or flake to rejection, where the system uses it.
9. Grout coat and topcoat(s).
10. Integral **cove base** where specified.
11. Cure time before traffic or service.

**By system**
- **Epoxy:**
  - Types: thin-film roll coat, self-leveling (about 1/16–1/8 in.), broadcast, mortar or trowel.
  - Watch for amine blush, recoat windows, and temperature and dew point limits.
- **Urethane cement:**
  - Commonly about **3/16–1/4 in.** for self-leveling and slurry systems, up to 3/8 in. for heavy-duty.
  - Used for thermal shock, food and beverage plants, and wet processing.
  - Needs **CSP 3–5** and keyways at all free edges.
  - Tolerates higher moisture than epoxy, per the manufacturer.
- **MMA (methyl methacrylate):**
  - Fast cure (about 1–2 hours, even in cold rooms).
  - Peroxide catalyst (BPO) dosed by temperature. Mix small batches.
  - Approved installers only (Sika, Sherwin-Williams Crylaflor, and others).
  - **Hazards:** strong odor and flammable vapors while uncured. The Sherwin-Williams guide calls for **negative-pressure, explosion-proof ventilation (about 12 air changes per hour)**, eliminating ignition sources, removing food from the space, and an OSHA vapor limit of 100 ppm.

**Standards:** the manufacturer system data sheet and installation guide; **ICRI 310.2R**; SSPC-SP 13 / NACE 6 (concrete prep for coatings); FeRFA *Guide to the Specification and Application of Synthetic Resin Flooring* (UK, widely referenced); ASTM D7234; and ASTM F2170 / F1869 per the manufacturer.

**Tools:** shot blaster, grinder with HEPA vacuum, saw for keyways, forced-action or drill mixer, gauge rake, notched squeegee, spiked roller, spiked shoes, broadcast hopper, a moisture meter and RH kit, a dew point and surface thermometer, an adhesion tester, and explosion-proof fans and a VOC monitor for MMA.

## 4. LVT / LVP: luxury vinyl tile and plank (CSI 09 65 19 resilient tile; product per ASTM F1700)
**Typical SOW**
1. Prep per §0.
2. Acclimate.
3. Lay out from the centerlines and balance the borders.
4. Apply the specified adhesive (pressure-sensitive or moisture-resistant) with the right trowel and open time. Click or loose-lay products follow the manufacturer.
5. Roll with a 100-lb roller (or the weight the manufacturer specifies).
6. Install transitions and base (09 65 13).
7. Protect the floor.
8. Initial maintenance per the manufacturer.

**Standards:** ASTM **F1700**, F710, F2170/F1869, the manufacturer guide; CFI resilient certification.

**Tools:** utility and hook knives, straightedge, 3- and 4-ft squares, laser or chalk line, notched trowels, 100-lb roller, hand roller, heat gun (for wraps), undercut saw, moisture and pH kits.

## 5. VCT: vinyl composition tile (CSI 09 65 19; product per ASTM F1066)
**Typical SOW**
1. Prep per §0.
2. Lay out with a quarter-turn or same-direction pattern per the spec.
3. Apply clear thin-spread or the manufacturer's adhesive.
4. Roll.
5. Install base.
6. **Initial maintenance:** clean, then apply multiple coats of floor finish after the manufacturer's wait time, typically several days. Strip and wax per the manufacturer.

**Standards:** ASTM **F1066**, F710, the manufacturer guide; CFI.

**Tools:** same as LVT, plus a floor machine and finish applicators.

## 6. Sheet vinyl and homogeneous / heterogeneous sheet (CSI 09 65 16; ASTM F1913 vinyl sheet without backing)
**Typical SOW**
1. Prep per §0.
2. Seam layout per the approved diagram (seams away from traffic and doors).
3. Full-spread adhesive.
4. Roll.
5. **Heat-weld seams** with a matching weld rod, then trim in two passes (or chemical seam sealing per the manufacturer).
6. **Flash cove** where specified: cove stick or fillet, cap strip, and inside and outside corners per the manufacturer.
7. Protect.

**Standards:** ASTM F1913, F710; the manufacturer's heat-welding and flash-cove guides (these govern, since there's no single consensus standard); CFI seam-welding certification.

**Tools:** hot-air welding gun with speed nozzle, groover, spatula or Mozart trimming knife, seam roller, scribers, cove former, 100-lb roller.

## 7. Rubber flooring: tile, sheet, stair treads (CSI 09 65 19.33 rubber tile; 09 65 16 sheet; 09 65 66 athletic)
**Typical SOW**
1. Prep per §0.
2. Acclimate (rubber is often more temperature-sensitive).
3. Apply the manufacturer's adhesive. Two-part urethane or epoxy is typical in wet or heavy-load areas.
4. Roll.
5. Weight seams or edges if the manufacturer requires it.
6. Stair treads use a nosing adhesive and caulk.
7. Clean with the manufacturer's maintenance products. Some rubber floors ban finish.

**Standards:** ASTM **F1859** (sheet without backing), **F1860** (sheet with backing), F1344-21a (rubber floor tile: homogeneous or layered; Class and Type designations not verified), F710, the manufacturer guide.

**Tools:** same as resilient, plus two-part adhesive mixing tools and weights or sandbags.

## 8. Carpet: carpet tile and broadloom (CSI 09 68 13 tile carpeting; 09 68 16 sheet carpeting)
**Typical SOW**
1. Prep per §0. Carpet adhesives also have moisture and pH limits.
2. Lay out per the installation method (monolithic, quarter-turn, ashlar, brick).
3. **Carpet tile:** pressure-sensitive adhesive or the manufacturer's tabs or "dots."
4. **Broadloom:** direct glue-down, double glue-down over cushion, or stretch-in over pad with tackless strip and a power stretcher.
5. Seam per the manufacturer (seam sealer on the cut edges).
6. Install transitions and base.
7. Vacuum and protect.

**Standards:** **CRI 104** (commercial installation), CRI 105 (residential), the manufacturer guide; CFI carpet certification; INSTALL (union) training, for UBC members only.

**Tools:** carpet knife, row cutter, seam iron and tape (broadloom), power stretcher and knee kicker, wall trimmer, stair tool, notched or roller adhesive applicator, roller.

## 9. Ceramic, porcelain, and stone floor tile (CSI 09 30 13 ceramic tiling; 09 30 16 quarry; 09 30 33 stone)
**Typical SOW**
1. Prep per §0.
2. Confirm the flatness tolerance (LFT, any edge 15 in.+: 1/8 in. in 10 ft and 1/16 in. in 2 ft, per A108.02 as quoted by CTEF).
3. Choose the TCNA Handbook method for the substrate and service, plus waterproofing (ANSI A118.10) or crack isolation (A118.12) where specified.
4. Lay out and balance the cuts.
5. Choose the mortar per ANSI A118.4/A118.15 (LFT mortar where needed).
6. Set with the right trowel and back-buttering. Coverage: **80% minimum, 95% for exterior or shower installations** (ANSI A108.5 §3.3.2 as quoted by CTEF; that quote is from the 2017 edition, and the current 2023 text wasn't viewed).
7. Movement joints per TCNA **EJ171**.
8. Grout per A118.6/A118.7, or epoxy grout per A118.3.
9. Seal the grout if specified.
10. Protect the floor and keep traffic off until cured.

**Standards:** **TCNA Handbook** (2026 ed.), **ANSI A108/A118/A137.1**, ANSI A326.3 (DCOF); CTEF **CTI/ACT**.

**Tools:** wet saw, snap cutter, notched trowels, leveling clips and wedges, margin trowel, grout float and sponges, mixing drill, laser.

## 10. Terrazzo: epoxy thin-set and cementitious (CSI 09 66 23.16 epoxy terrazzo; 09 66 13 portland cement terrazzo)
**Typical SOW (epoxy)**
1. Prep and moisture testing per the NTMA and the manufacturer.
2. Crack isolation membrane at cracks and joints.
3. Primer.
4. Install divider strips per the design. Joint strips go at slab control joints.
5. Place the epoxy matrix with aggregate, nominal **3/8 in.** (NTMA).
6. Cure.
7. Grind in stages.
8. Grout the voids.
9. Fine grind and polish.
10. Seal.

**Cementitious** systems (sand cushion, bonded, monolithic) are thicker and follow NTMA details.

**Standards:** **NTMA** specifications and technical guides; the manufacturer's epoxy system data.

**Tools:** terrazzo grinders (wet), divider-strip tools, mixers, trowels and screeds, vacuums. This is usually a specialty contractor (NTMA member).

## 11. Wood and engineered wood (CSI 09 64 00 wood flooring; 09 64 66 athletic wood)
**Typical SOW (per the NWFA Installation Guidelines)**
1. Jobsite conditions:
   - Building enclosed.
   - HVAC running (NWFA calls for it operating about 5 days before delivery).
   - Interior about 60–80°F and 30–50% RH, or as the manufacturer specifies.
2. Test the wood and subfloor moisture: a pin or pinless meter for wood and wood subfloors, and RH or MVER on concrete per the manufacturer.
3. Choose the method for the product and subfloor:
   - **Nail-down:** solid or engineered over wood.
   - **Glue-down:** often engineered over concrete, with a moisture-retarder adhesive.
   - **Floating.**
4. Vapor retarder per the NWFA and manufacturer.
5. Expansion space at the perimeter.
6. Rack and stagger the end joints.
7. Site-finished floors: sand through grit sequences, stain, and apply finish coats.
8. Install transitions and thresholds.

**Standards:** **NWFA Installation Guidelines** (2025 rev.) and *Sand and Finish Guidelines*; the manufacturer; NWFA Certified Installer / Sand & Finisher.

**Tools:** flooring nailer and stapler, compressor, miter and table saws, wood moisture meter, RH kit, drum or belt and edger sanders, buffer, finish applicators.

---

## Cross-type quick table
| Type | CSI (typical) | Key standard(s) | Installer credential |
|---|---|---|---|
| Polished concrete | 03 35 43 | ACI 310.1, CPC, ICRI 310.2R | ASCC CPC |
| Grind and seal | 03 35 43 (reduced) | Same | ASCC CPC |
| Epoxy / urethane cement / MMA | 09 67 23 | Manufacturer system, ICRI 310.2R, SSPC-SP 13 | Manufacturer-approved applicator |
| LVT/LVP | 09 65 19 | ASTM F1700, F710 | CFI |
| VCT | 09 65 19 | ASTM F1066, F710 | CFI |
| Sheet vinyl | 09 65 16 | ASTM F1913, F710, manufacturer weld/cove | CFI (seam welding) |
| Rubber | 09 65 19.33 / 09 65 16 | ASTM F1859/F1860, F710 | CFI, manufacturer |
| Carpet tile / broadloom | 09 68 13 / 09 68 16 | CRI 104 | CFI, INSTALL |
| Ceramic/porcelain/stone | 09 30 13 | TCNA Handbook, ANSI A108/A118 | CTEF CTI/ACT |
| Terrazzo | 09 66 23.16 / 09 66 13 | NTMA | NTMA contractor |
| Wood / engineered | 09 64 00 | NWFA Guidelines | NWFA CP |
| All: floor prep | 09 05 61 / 03 54 | ASTM F710, F2170, F1869, ICRI 310.2R | — |
