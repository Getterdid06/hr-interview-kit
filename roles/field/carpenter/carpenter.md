# Role: Carpenter: Rough (Formwork, Framing, Blocking, Temp Protection) and Finish (Trim, Millwork, Doors)

Answer key: `answer-keys/field/carpenter/carpenter-KEY.md`
Trade group: **Carpenter**.

Benchmarks:
- **NCCER Carpentry** (Carpentry Framing & Finishing) and the Concrete Finisher formwork domains.
- **OSHA Subpart M** (fall protection) and **Subpart Q** (concrete and formwork).
- **Finish carpentry:**
  - **ANSI/AWI 0620-2018** *Finish Carpentry/Installation*. It replaced the installation section of the AWI *Architectural Woodwork Standards*, 2nd Ed.
  - **AWI quality grades:** Economy, Custom, Premium.
  - **NFPA 80** for rated doors.
  - **2010 ADA Standards** for door hardware and clear widths.

**Related files:**
- Metal stud framing and drywall: `roles/field/drywall/drywall-metal-framing.md`
- Doors, hardware, and Division 10 specialties at installer depth: `roles/field/finishes/finishes-installer.md`

## Position tuning
```yaml
position_title: Carpenter     # Helper | Carpenter | Lead Carpenter
seniority: mid                  # entry | mid | senior (thresholds: 01 §4)
delivery: self-perform          # self-perform | sub-managed | both. Default self-perform: the company can self-perform every listed scope, so hands-on skill is scored.
sub_coordination_qa: off        # turn on when the job is subbed; the interviewer then weights coordination and QA over hands-on skill (document it in weights)
scope: [rough, finish]          # turn off whichever the job doesn't need
work_types: [slab repair forms, curbs/pads, wood/metal stud framing, blocking for LV devices/accessories/casework, temp walls/dust barriers, floor protection, base/casing/trim, casework & countertops, door hang & hardware]
license_required: n/a
must_have_certs: [OSHA 10]
nice_to_have: [NCCER Carpentry, OSHA 30]
interview_length_min: 35
sections: {A_trade_skill: on, B_safety: on, C_quality: on, G_finish_carpentry: on, D_field_tech_module: on, E_core: on, F_skills_demo: on}
knockouts: [disregards fall protection, falsified certs]
weights: equal   # 01 §4 default; document a reason if changed
notes_for_today: ""
```

## A. Trade skill (rough carpentry)
| ID | Type | Question |
|---|---|---|
| CAR-A1 ★ | B | "Tell me about the last formwork job you built: what it was, how you set grade and line, and how you braced it." |
| CAR-A2 ★ | T | "How do you square a layout with just a tape?" |
| CAR-A3 | T | "Read this plan detail and tell me what you'd build." (provide a curb or pad detail) |
| CAR-A4 | T | "How do you frame and block a wall to hold a wall-mounted controller or TV?" |
| CAR-A5 | T | "What laser or layout tools have you used? How do you check a laser is accurate?" |

## B. Safety
| ID | Type | Question |
|---|---|---|
| CAR-B1 ★ | T | "At what height do you need fall protection in construction, and what are your options?" |
| CAR-B2 | T | "What saw safety habits do you follow with a circular saw and a miter saw?" |

## C. Quality
| ID | Type | Question |
|---|---|---|
| CAR-C1 | B | "Tell me about a time something you built was out of tolerance. How did you find it and fix it?" |

## G. Finish carpentry (if `scope` includes finish)
| ID | Type | Question |
|---|---|---|
| CAR-G1 ★ | B | "Walk me through installing a run of plastic-laminate base cabinets and upper cabinets in a break room, from layout to final adjustment." |
| CAR-G2 | T | "How do you cope or miter inside and outside corners on base and crown so the joints stay tight?" |
| CAR-G3 ★ | T | "Hanging a pre-hung or slab door in a hollow metal frame: what do you check for clearances, hardware, and swing?" |
| CAR-G4 | T | "What's different about installing a fire-rated door assembly?" |
| CAR-G5 | T | "The spec calls for AWI Custom grade. What does that tell you about the work?" |
| CAR-G6 | S | "Casework arrives damaged, or the field dimensions don't match the shop drawings. What do you do?" |

## D. Field tech module
Add questions from `roles/field/field-tools-tech-module.md` (FT-1 to FT-6). Score them with its key.

## E. Core
Ask questions from `03-common-core-questions.md` (field variant), per `00-system-prompt.md` §3.

## F. Skills demo
| ID | Type | Question |
|---|---|---|
| CAR-F | W | Skills demo (rough): build a small square box frame, or lay out a 6' × 8' rectangle square within 1/8". Skills demo (finish): cope an inside base corner and miter an outside corner, or set a door and hardware to the stated clearances. |
