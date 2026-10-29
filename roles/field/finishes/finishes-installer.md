# Role: Finishes Installer: Ceilings (ACT), Wall Tile, Millwork/Trim, Doors/Frames/Hardware, Division 10 Specialties, Wall Coverings

Answer key: `answer-keys/field/finishes/finishes-installer-KEY.md`
Trade group: **Finishes**.

Related files:
- **Floor** finishes (including floor tile, terrazzo, resilient, carpet, wood, coatings, and polished concrete) are in `roles/field/flooring/`.
- Painting is in `roles/field/painter/`.
- Rough and finish carpentry at depth is in `roles/field/carpenter/`.

## Benchmarks (verify current editions per `update-checklist.md`)

**CSI MasterFormat**
- **Division 09, Finishes:**
  - 09 30 00: tiling (09 30 13 ceramic)
  - 09 51 00: acoustical ceilings (09 51 13 acoustical panel)
  - 09 53 00: acoustical ceiling suspension
  - 09 72 00: wall coverings
- Related divisions: **Division 06, Wood, Plastics, and Composites**; **Division 08, Openings**; **Division 10, Specialties** (division titles confirmed in CSI's MasterFormat guide, 2026). The section numbers below are standard MasterFormat but weren't confirmed against a 2026 list, so confirm them against the project manual:
  - **06 20 00:** finish carpentry
  - **06 40 00:** architectural woodwork
  - **06 64 00:** plastic paneling (FRP)
  - **08 11 00:** hollow metal doors and frames
  - **08 14 00:** wood doors
  - **08 71 00:** door hardware
  - **10 14 00:** signage
  - **10 21 00:** toilet compartments
  - **10 28 00:** toilet, bath, and laundry accessories
  - **10 44 00:** fire protection specialties

**Ceilings**
- **ASTM C636:** installation of metal ceiling suspension systems.
- **ASTM E580:** installation in seismic areas (with ASCE 7).
- **CISCA Seismic Construction Handbook.**

**Tile**
- **TCNA Handbook for Ceramic, Glass, and Stone Tile Installation.** The 2026 edition is current.
- **ANSI A108/A118/A136/A137** standards.
- **CTEF** installer credentials: Certified Tile Installer (CTI) and Advanced Certifications for Tile Installers (ACT).

**Millwork, doors, and accessibility**
- **ANSI/AWI 0620-2018**, *Finish Carpentry/Installation*. Covers AWI grades.
- **NFPA 80**, fire doors.
- **DHI:** AHC (Architectural Hardware Consultant) and CFDAI (fire and egress door assembly inspector).
- **2010 ADA Standards** for mounting heights and door hardware.

## Position tuning
```yaml
position_title: Finishes Installer        # Helper | Installer | Lead | Specialty (ceilings | tile setter | door/hardware | Div 10)
seniority: mid                  # entry | mid | senior (thresholds: 01 §4)
delivery: self-perform          # self-perform | sub-managed | both. Default self-perform: the company can self-perform every listed scope, so hands-on skill is scored.
sub_coordination_qa: off        # turn on when the job is subbed; the interviewer then weights coordination and QA over hands-on skill (document it in weights)
work_types: n/a   # see sub_specialties
sub_specialties: [CL_ceilings, TL_wall_tile, MW_millwork, DR_doors_hardware, SP_div10_specialties, WC_wall_coverings]   # turn on only what the job needs; each maps to a section toggle
project_types: ["?"]      # e.g., office TI, healthcare, K-12, retail; ask
seismic_design_category: "?"   # matters for ceilings (ASTM E580); ask the PM/structural drawings
license_required: n/a
must_have_certs: [OSHA 10]
nice_to_have: [CTEF CTI/ACT, DHI AHC/CFDAI, NCCER Carpentry, MEWP training]
interview_length_min: 40
sections: {B_safety: on, CL_ceilings: on, TL_wall_tile: off, MW_millwork: off, DR_doors_hardware: on, SP_div10_specialties: on, WC_wall_coverings: off, D_field_tech_module: on, E_core: on, F_skills_demo: on}
knockouts: [field-modifies labeled fire door/frame, hangs ceiling/fixtures from ducts/pipe, falsified certs]
weights: equal   # 01 §4 default; document a reason if changed
notes_for_today: ""
```

## B. Safety
| ID | Type | Question |
|---|---|---|
| FIN-B1 ★ | T | "Working above ceilings on a ladder or lift: what do you watch for?" |
| FIN-B2 | T | "Cutting tile, stone, or cement board: how do you control silica dust?" |

## CL. Acoustical ceilings (ACT)
| ID | Type | Question |
|---|---|---|
| FIN-CL1 ★ | B | "Walk me through laying out and installing a 2×2 ACT ceiling in an office from the reflected ceiling plan." |
| FIN-CL2 ★ | T | "How do you hang the grid: wire size, spacing, splay, and what you attach to?" |
| FIN-CL3 | T | "What changes in a seismic area?" |
| FIN-CL4 | S | "The ductwork is right where your hanger wire needs to go. What do you do?" |

## TL. Wall tile (floor tile is in Flooring)
| ID | Type | Question |
|---|---|---|
| FIN-TL1 ★ | T | "Tiling a shower wall: what's behind the tile, and how do you waterproof it?" |
| FIN-TL2 | T | "How do you get proper mortar coverage, and how do you check it?" |
| FIN-TL3 | T | "Where do movement joints go in tile, and what goes in them?" |

## MW. Millwork and trim
| ID | Type | Question |
|---|---|---|
| FIN-MW1 | T | "Installing casework and countertops to AWI Custom grade: what do you check?" (Use `roles/field/carpenter/` CAR-G for depth.) |

## DR. Doors, frames, and hardware
| ID | Type | Question |
|---|---|---|
| FIN-DR1 ★ | T | "Setting a hollow metal frame in a drywall partition: how do you anchor it and keep it plumb and square?" |
| FIN-DR2 ★ | T | "How do you read a hardware schedule, and what do you check when you install a set?" |
| FIN-DR3 ★ | T | "What can and can't you do to a fire-rated door, frame, or hardware in the field?" |

## SP. Division 10 specialties
| ID | Type | Question |
|---|---|---|
| FIN-SP1 ★ | T | "Installing toilet accessories and grab bars in an accessible restroom: what heights and clearances do you check?" |
| FIN-SP2 | T | "Installing toilet partitions: what's the sequence, and how do you anchor them?" |
| FIN-SP3 | T | "Signage, fire extinguisher cabinets, and corner guards: where does mounting information come from?" |

## WC. Wall coverings and FRP
| ID | Type | Question |
|---|---|---|
| FIN-WC1 | T | "How do you install FRP panels in a kitchen or janitor closet?" |

## D. Tools and tech
| ID | Type | Question |
|---|---|---|
| FIN-D1 | B | "Which tools do you use: rotary or line lasers, wet saws, hardware templates and jigs, powder-actuated tools, RCP and shop-drawing apps?" |

## E. Core
Ask questions from `03-common-core-questions.md` (field variant), per `00-system-prompt.md` §3.

## F. Skills demo
Pick one per enabled sub-specialty:
- Set a level grid line with a laser.
- Back-butter and set tile, then pull it to show coverage.
- Install a lever set and a closer per the template.
- Mark accessory heights on a mock wall from an ADA elevation.
