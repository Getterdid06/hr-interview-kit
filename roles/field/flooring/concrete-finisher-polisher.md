# Role: Concrete Polisher / Grinder / Finisher (Polish and Grind-and-Seal)

Answer key: `answer-keys/field/flooring/concrete-finisher-polisher-KEY.md`
Trade group: **Flooring**. Multi-type flooring roles: `flooring-installer.md`. Scope and SOW by type: `flooring-scope-reference.md`.
Benchmarks:
- **ASCC Concrete Polishing Council (CPC):** Tradesman certification (50-question exam) and Craftsman certification (Tradesman plus 4,500 verified hours). Knowledge areas: planning, surface prep, grinding, edging, chemical application, honing, polishing, equipment maintenance, safety.
- **ACI/ASCC 310.1-20** polished concrete specification.
- **ICRI 310.2R** concrete surface profiles (CSP 1–10).
- **NCCER Concrete Finisher** journey-level assessment.
- **OSHA 1926.1153** (silica).

## Position tuning
```yaml
position_title: Concrete Polisher     # Helper | Operator | Lead Polisher | Finisher (placement)
seniority: mid                         # entry/helper | mid/operator | senior/lead
delivery: self-perform          # self-perform | sub-managed | both. Default self-perform: the company can self-perform every listed scope, so hands-on skill is scored.
sub_coordination_qa: off        # turn on when the job is subbed; the interviewer then weights coordination and QA over hands-on skill (document it in weights)
work_types: [polish, grind_and_seal, coating_prep, joint_fill]   # add placement_finishing if hiring finishers
machines_we_run: ["?"]                 # e.g., HTC, Husqvarna, Lavina, SASE, propane burnishers; ask the hiring manager
travel_overnight: "?"                  # ask; don't assume
license_required: n/a
must_have_certs: []                    # e.g., OSHA 10 card; driver's license if driving the company truck
nice_to_have: [ASCC CPC Tradesman/Craftsman, NCCER Concrete Finisher, OSHA 10/30]
interview_length_min: 40
sections: {A_trade_skill: on, B_safety: on, C_quality: on, D_field_tech_module: on, E_core: on, F_skills_demo: on}
knockouts: [refuses silica controls/respirator when required, unsafe propane use indoors, falsified hours/certs]
weights: equal   # 01 §4 default; document a reason if changed
notes_for_today: ""
```

## A. Trade skill
| ID | Type | Question |
|---|---|---|
| POL-A1 ★ | B | "Walk me through a polish job you ran or worked on, from arrival to final pass. What grits, in what order, and when did the densifier go down?" |
| POL-A2 ★ | T | "How do you pick the diamond bond for a slab? What happens if you get it wrong?" |
| POL-A3 | T | "How do you know you're ready to go to the next grit?" |
| POL-A4 | T | "What's the difference between a Class A, B, and C exposure? How does it change how you start the job?" |
| POL-A5 ★ | S | "You arrive and the slab has old mastic in one area and sealer in another. How do you find out, and what do you do?" |
| POL-A6 | T | "How do you handle edges, columns, and joints? What joint filler have you used, and when do you install it?" |
| POL-A7 | T | "What's the difference between a grind-and-seal and a polish? What sealers or guards have you applied, and how?" |
| POL-A8 | T | "What daily maintenance do you do on the grinder, vacuum, and tooling?" |
| POL-A9 (lead) | B | "How have you set up a crew's production on a large floor? How much did you get done per day and why?" |

## B. Safety
| ID | Type | Question |
|---|---|---|
| POL-B1 ★ | T | "Grinding concrete makes silica dust. How do you control it on the job?" |
| POL-B2 | T | "What do you watch for running propane equipment indoors?" |
| POL-B3 | S | "Your vacuum filter keeps clogging and the air is getting dusty, but the GC wants you done today. What do you do?" |

## C. Quality
| ID | Type | Question |
|---|---|---|
| POL-C1 | T | "How do you check a finished polished floor against the spec (shine, clarity, scratches)?" |
| POL-C2 | B | "Tell me about a floor that didn't come out right. What happened and how did you fix it?" |

## D. Field tech (from `field-tools-tech-module.md`)
Pick 2: FT-1 to FT-6.

## E. Core
Pick 2: CORE-1, CORE-2, CORE-3 (field variants).

## F. Skills demo (optional, 15–20 min, paid if your policy says so)
Have the candidate inspect a sample or mock-up slab area and:
1. do a water-drop test for existing sealer
2. pick tooling for a hardness test result you give them
3. run the edger or grinder for 2 minutes with dust extraction on
4. inspect a scratch pattern with a low-angle light

Score 1–5 using the anchors in the key.
