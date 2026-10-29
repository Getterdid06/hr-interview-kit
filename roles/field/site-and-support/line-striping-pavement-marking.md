# Role: Line Striping / Pavement Marking Technician

Answer key: `answer-keys/field/site-and-support/line-striping-pavement-marking-KEY.md`
Benchmarks:
- **MUTCD 11th Edition (2023), Part 3:** longitudinal lines 4–6 in. wide; wide lines at least twice the normal width.
- **MUTCD Part 6:** temporary traffic control.
- **2010 ADA Standards §502:** accessible parking.
- **ATSSA:** Pavement Marking Technician (PMT) and Flagger certifications.
- **State DOT pavement marking manuals** (e.g., TDOT) for public roads.

## Position tuning
```yaml
position_title: Striping Technician   # Helper | Striper/Operator | Striping Lead
seniority: mid                  # entry | mid | senior (thresholds: 01 §4)
delivery: self-perform          # self-perform | sub-managed | both. Default self-perform: the company can self-perform every listed scope, so hands-on skill is scored.
sub_coordination_qa: off        # turn on when the job is subbed; the interviewer then weights coordination and QA over hands-on skill (document it in weights)
work_types: [parking_lot_restripe, new_layout, ADA, warehouse_floor_lines, road/DOT]
materials_we_use: [waterborne paint, ?thermoplastic, ?epoxy/MMA, glass beads]
equipment_we_use: ["?"]               # e.g., Graco LineLazer, ride-on striper; ask
license_required: n/a
must_have_certs: [valid driver's license if driving truck/trailer]
nice_to_have: [ATSSA PMT, ATSSA Flagger, OSHA 10]
interview_length_min: 35
sections: {A_trade_skill: on, B_safety_traffic: on, C_quality: on, D_field_tech_module: on, E_core: on, F_skills_demo: on}
knockouts: [unsafe traffic exposure behavior, falsified certs]
weights: equal   # 01 §4 default; document a reason if changed
notes_for_today: ""
```

## A. Trade skill
| ID | Type | Question |
|---|---|---|
| STR-A1 ★ | B | "Walk me through a parking lot restripe from arrival to opening the lot back up." |
| STR-A2 ★ | T | "How do you lay out a new lot with no existing lines? What tools do you use?" |
| STR-A3 ★ | T | "What are the size rules for an accessible (ADA) stall and a van-accessible stall?" |
| STR-A4 | T | "What weather and surface conditions stop you from painting?" |
| STR-A5 | T | "How do you set up and maintain your striper (tips, pressure, filters, beads)? How thick do you put paint down?" |
| STR-A6 | S | "The note says 'remove conflicting markings.' How do you do that, and what shouldn't you do?" |
| STR-A7 | T | "About how much 4-inch line will a gallon of paint do at 15 mils wet? How would you figure it?" (lead/mid) |

## B. Safety and traffic
| ID | Type | Question |
|---|---|---|
| STR-B1 ★ | S | "You're striping in an open lot with cars moving. How do you protect yourself and the crew?" |

## C. Quality
| ID | Type | Question |
|---|---|---|
| STR-C1 | B | "Tell me about a striping job that had a problem (overspray, tracking, crooked line). What did you do?" |

## D. Field tech module
| ID | Type | Question |
|---|---|---|
| STR-D/E | — | FT-1, FT-3, FT-4 + CORE-2. |

## E. Core
CORE-2 is listed in the STR-D/E row under D.

## F. Skills demo
| ID | Type | Question |
|---|---|---|
| STR-F | W | Skills demo: snap a 40-ft straight line and lay out two 9-ft stalls with a tape and chalk; or run a test line on cardboard or scrap. |
