# Role: Flooring Installer (Multi-Type), with a Floor-Type Selector

Answer key: `answer-keys/field/flooring/flooring-installer-KEY.md`
Trade group: **Flooring**.

Related files:
- **Scope reference** (SOW, standards, and tools by type): `roles/field/flooring/flooring-scope-reference.md`. Read it before tuning.
- **Polished concrete and grind-and-seal at full depth:** `roles/field/flooring/concrete-finisher-polisher.md`. Use it instead of section POL here when polish is the main scope.

## Benchmarks
- Manufacturer installation instructions govern. After those, the standards in the scope reference:
  - ASTM F710, F2170, and F1869
  - ICRI 310.2R
  - ASTM F1700, F1066, F1913, F1859, and F1860
  - CRI 104
  - TCNA Handbook and ANSI A108/A118
  - NTMA
  - NWFA Installation Guidelines
  - ACI 310.1 and CPC
- **Certifications:**
  - CFI (resilient, seam welding, carpet)
  - NWFA Certified Installer
  - CTEF CTI/ACT (tile)
  - ASCC CPC (polish)
  - INSTALL (union floorcovering; available only to UBC carpenters' union members, so it's not a must-have for non-union installers)
  - Not an installer cert: FCICA CIM (Certified Installation Manager) is a PM or manager credential for commercial flooring projects. Use it for PM or manager roles, not to score installers.
  - Manufacturer-approved applicator (resinous, MMA)

## Position tuning
Floor types: set `floor_types:`; PREP is always on.
```yaml
position_title: Flooring Installer        # Helper | Installer | Lead | Foreman | Floor Prep Tech
seniority: mid                  # entry | mid | senior (thresholds: 01 §4)
delivery: self-perform          # self-perform | sub-managed | both. Default self-perform: the company can self-perform every listed scope, so hands-on skill is scored.
sub_coordination_qa: off        # turn on when the job is subbed; the interviewer then weights coordination and QA over hands-on skill (document it in weights)
work_types: n/a   # see floor_types
floor_types:            # turn on every type the position covers; each maps to a section below
  PREP_floor_prep: on               # always on: moisture, pH, CSP, leveling
  POL_polished_concrete: off
  GS_grind_and_seal: off
  RES_epoxy_resinous: off           # epoxy, urethane cement
  MMA_methyl_methacrylate: off
  LVT_lvt_lvp: on
  VCT_vct: off
  SV_sheet_vinyl_heat_weld: off
  RUB_rubber: off
  CPT_carpet_tile_broadloom: off
  TILE_ceramic_porcelain_stone: off
  TZ_terrazzo: off
  WD_wood_engineered: off
project_types: ["?"]              # e.g., healthcare, K-12, retail, food plant, warehouse, multifamily; ask
license_required: n/a
must_have_certs: [OSHA 10]
nice_to_have: [CFI, NWFA CP, CTEF CTI, ASCC CPC, manufacturer applicator approval, INSTALL]   # INSTALL = UBC union members only
interview_length_min: 45          # ~8–10 min per enabled type + prep + core
sections: {B_safety: on, D_field_tech_module: on, E_core: on, F_skills_demo: on}
knockouts: [installs over failed/untested moisture without approval, disturbs suspect asbestos flooring/mastic without testing, unsafe MMA/solvent ventilation, falsified certs]
weights: equal   # 01 §4 default; document a reason if changed
notes_for_today: ""
```
**Rule.** Ask every ★ question in each enabled section. If more than 3 types are enabled, ask only the ★ items for the extra types to fit the time.

## B. Safety (always on)
| ID | Type | Question |
|---|---|---|
| FLR-B1 ★ | T | "Grinding, shot blasting, or cutting concrete or tile: how do you control silica?" |
| FLR-B2 | T | "How do you protect your knees, back, and lungs on a long install?" |
| FLR-B3 | T | "Working with solvent-based adhesives or resins: what do you need on site?" |

## PREP. Floor prep (always on)
| ID | Type | Question |
|---|---|---|
| FLR-PREP1 ★ | T | "Before you glue down a resilient floor on a concrete slab, what tests do you run, how, and who sets the pass/fail number?" |
| FLR-PREP2 ★ | T | "The slab has cracks, old adhesive, and a low spot. Walk me through getting it ready." |
| FLR-PREP3 ★ | S | "You're tearing out old 9×9 tile with black mastic. What do you do first?" |
| FLR-PREP4 | T | "When do you use a self-leveler, and how do you install it?" |
| FLR-PREP5 | T | "What does CSP mean, and how do you get the CSP a system needs?" |

## POL / GS. Polished concrete and grind-and-seal
| ID | Type | Question |
|---|---|---|
| FLR-POL1 ★ | T | "What's the difference in scope between a full polish and a grind-and-seal?" (For depth, use POL-A1/A2 from `concrete-finisher-polisher.md`.) |

## RES. Epoxy and resinous (including urethane cement)
| ID | Type | Question |
|---|---|---|
| FLR-RES1 ★ | B | "Walk me through a broadcast epoxy or urethane cement floor you installed, from prep to topcoat." |
| FLR-RES2 ★ | T | "Why do urethane cement floors need keyways, and where do they go?" |
| FLR-RES3 | T | "What can go wrong with temperature, dew point, or moisture during an epoxy install?" |
| FLR-RES4 | T | "How do you install an integral cove base?" |

## MMA. Methyl methacrylate
| ID | Type | Question |
|---|---|---|
| FLR-MMA1 ★ | T | "What's different about installing MMA compared to epoxy: safety, mixing, and timing?" |

## LVT. LVT and LVP
| ID | Type | Question |
|---|---|---|
| FLR-LVT1 ★ | B | "Walk me through a glue-down LVT install in a 5,000 SF office, from acclimation to protection." |
| FLR-LVT2 | T | "How do you pick the trowel and work the adhesive open time?" |
| FLR-LVT3 | T | "Where do you start the layout, and how do you avoid slivers at doorways?" |

## VCT
| ID | Type | Question |
|---|---|---|
| FLR-VCT1 ★ | T | "How do you install VCT and turn it over? When does floor finish go on?" |

## SV. Sheet vinyl and heat welding
| ID | Type | Question |
|---|---|---|
| FLR-SV1 ★ | T | "Walk me through heat-welding a seam in homogeneous sheet vinyl." |
| FLR-SV2 | T | "How do you build a flash cove at an inside corner?" |

## RUB. Rubber
| ID | Type | Question |
|---|---|---|
| FLR-RUB1 ★ | T | "What's different about installing rubber tile or sheet, including adhesives and conditions?" |

## CPT. Carpet tile and broadloom
| ID | Type | Question |
|---|---|---|
| FLR-CPT1 ★ | T | "Carpet tile versus broadloom: how does the install differ? What do you check before you start?" |
| FLR-CPT2 | T | "Stretch-in broadloom: what tools do you use, and how do you make a seam disappear?" |

## TILE. Ceramic, porcelain, and stone floor tile
| ID | Type | Question |
|---|---|---|
| FLR-TILE1 ★ | T | "Setting 24×48 porcelain on a slab: flatness, mortar, coverage, and movement joints?" |
| FLR-TILE2 | T | "How do you pick the TCNA method for the job?" |

## TZ. Terrazzo
| ID | Type | Question |
|---|---|---|
| FLR-TZ1 ★ | T | "Walk me through an epoxy terrazzo install. Where do the divider strips go?" |

## WD. Wood and engineered
| ID | Type | Question |
|---|---|---|
| FLR-WD1 ★ | T | "Before you install wood flooring, what site conditions and moisture readings do you need?" |
| FLR-WD2 | T | "Nail-down, glue-down, or floating: how do you choose, and what's different about each?" |

## D. Tools and tech
| ID | Type | Question |
|---|---|---|
| FLR-D1 | B | "Which testing and layout tools and apps do you use: RH probe readers and logging apps, lasers, moisture meters, CAD seam diagrams, photo logs?" |

## E. Core
Ask questions from `03-common-core-questions.md` (field variant), per `00-system-prompt.md` §3.

## F. Skills demo
Pick one per enabled type:
- **Prep:** read a set of RH readings and a manufacturer limit and make the call.
- **LVT/VCT:** lay out and set a small field square to a line.
- **Sheet:** weld and trim a seam on a scrap.
- **Tile:** set a tile, pull it, and show the coverage.
- **Resinous:** state the mix ratio and pot life from the data sheet.
