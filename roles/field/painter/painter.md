# Role: Painter: Commercial Painting, Coatings, Wall Coverings, Surface Prep

Answer key: `answer-keys/field/painter/painter-KEY.md`
Trade group: **Painter**.

## Benchmarks (verify current editions per `update-checklist.md`)

**Surface prep (SSPC/AMPP, for steel)**
- **SP 1:** solvent cleaning
- **SP 2:** hand tool
- **SP 3:** power tool
- **SP 6:** commercial blast
- **SP 10:** near-white blast
- **SP 15:** commercial grade power tool to bare metal
- **SSPC-SP 13 / NACE 6:** concrete surface prep

**Measurement and industry standards**
- **SSPC-PA 2:** measuring dry film thickness.
- **PCA (Painting Contractors Association, formerly PDCA) Industry Standards:** published with the FCA. Cover touch-up, levels of finish expectations, and inspection lighting.
- **MPI** paint systems, where the spec references them.

**Lead**
- **EPA RRP Rule (40 CFR 745 Subpart E)** applies to renovation that disturbs paint in **pre-1978 housing and child-occupied facilities**, including portions of commercial buildings that are child-occupied facilities. It requires a certified firm and a certified renovator. It doesn't cover ordinary commercial work.
- **OSHA 29 CFR 1926.62** (lead in construction) applies to any construction exposure. PEL 50 µg/m³ (8-hr TWA); action level 30 µg/m³.

**CSI sections**
- 09 91 00: painting
- 09 96 00: high-performance coatings
- 09 72 00: wall coverings

**Training and certifications**
- IUPAT / Finishing Trades Institute apprenticeship.
- NCCER Painting.
- AMPP coating inspector (CIP), for high-performance work leads.

## Position tuning
```yaml
position_title: Painter        # Helper/Prep | Journeyman Painter | Industrial/High-Performance Coatings | Wall covering hanger | Lead
seniority: mid                  # entry | mid | senior (thresholds: 01 §4)
delivery: self-perform          # self-perform | sub-managed | both. Default self-perform: the company can self-perform every listed scope, so hands-on skill is scored.
sub_coordination_qa: off        # turn on when the job is subbed; the interviewer then weights coordination and QA over hands-on skill (document it in weights)
work_types: [interior commercial repaint, new construction, occupied/healthcare, exterior, high-performance (epoxy/urethane), steel/structural, wall coverings, intumescent (spec-dependent)]
pre_1978_child_occupied_work: "?"     # if yes, RRP certified renovator required
license_required: n/a
must_have_certs: [OSHA 10]           # add EPA RRP Certified Renovator if the line above is yes
nice_to_have: [IUPAT/FTI, NCCER Painting, AMPP CIP, aerial/MEWP training, respirator fit test current]
interview_length_min: 40
sections: {A_trade_skill: on, B_safety: on, P_prep_and_coatings: on, W_wallcovering: off, L_lead: on, D_field_tech_module: on, E_core: on, F_skills_demo: on}
knockouts: [dry-sands/torches lead paint, skips respirator where required, falsified RRP/certs]
weights: equal   # 01 §4 default; document a reason if changed
notes_for_today: ""
```

## A. Trade skill
| ID | Type | Question |
|---|---|---|
| PNT-A1 ★ | B | "Walk me through painting an occupied office corridor from start to finish: prep, protection, products, coats, and turnover." |
| PNT-A2 ★ | T | "How do you read the paint schedule and spec? What has to match before you open a can?" |
| PNT-A3 | T | "When do you spray, roll, or brush? How do you set up and clean an airless sprayer?" |
| PNT-A4 | T | "What do you check about the weather and the surface before coating (temperature, humidity, dew point)?" |
| PNT-A5 | S | "The GC says the walls look patchy after your second coat. What causes that, and what do you do?" |

## B. Safety
| ID | Type | Question |
|---|---|---|
| PNT-B1 ★ | T | "What PPE and ventilation do you use when you spray solvent-based or isocyanate coatings?" |
| PNT-B2 | T | "Working from a ladder, scaffold, or lift: what rules do you follow?" |
| PNT-B3 | T | "How do you store and dispose of paint, rags, and solvents?" |

## P. Surface prep and coatings
| ID | Type | Question |
|---|---|---|
| PNT-P1 ★ | T | "The spec for structural steel calls for SSPC-SP 6 and an epoxy-urethane system. What does that mean on site?" |
| PNT-P2 | T | "How do you prepare new drywall, masonry, galvanized metal, and previously glossy surfaces?" |
| PNT-P3 | T | "How do you check film thickness (wet and dry), and why does it matter?" |
| PNT-P4 | T | "Working with a two-component epoxy or urethane: what's different?" |

## W. Wall coverings (turn on if needed)
| ID | Type | Question |
|---|---|---|
| PNT-W1 | T | "How do you prep, prime, and hang Type II vinyl wall covering, including pattern matching and seams?" |

## L. Lead and hazardous coatings
| ID | Type | Question |
|---|---|---|
| PNT-L1 ★ | T | "You're scraping paint in a building from the 1960s. What do you do before you start?" |
| PNT-L2 | T | "When does the EPA RRP rule apply, and what does a certified renovator do?" |

## D. Tools and tech
| ID | Type | Question |
|---|---|---|
| PNT-D1 | B | "Which tools do you use: airless sprayers, HVLP, DFT and WFT gauges, moisture meters, dew-point meters, color-matching apps, punch-list apps?" |

## E. Core
Ask questions from `03-common-core-questions.md` (field variant), per `00-system-prompt.md` §3.

## F. Skills demo
Pick one:
- Cut in and roll a 4×8 panel with a clean line and no lap marks.
- Read a coating data sheet and give the recoat window, the DFT, and the minimum surface temperature.
